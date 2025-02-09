<template>
  <div class="card mt-3">
    <div class="card-body">
      <div class="d-flex justify-content-between">
        <span class="color-blue nomination-header">Nomination Status</span>
        <img src="../../assets/up_arrow.svg" alt="up_arrow" />
      </div>
      <hr />
      <label class="color-grey label-font">Project:</label>
      <p>Alzheimer P2P 2023</p>
      <label class="color-grey label-font">Brand:</label>
      <p>Vitiligo 2023</p>
      <label class="color-grey label-font">New/Re-nominated</label><br />
      <span class="badge new-badge" style="">New</span>
      <hr />
      <ul class="nomination-ul-list">
        <li>
          <img src="../../assets/check.svg" alt="checks" />
          <span class="ms-4 color-green">Screening</span>
          <p class="ms-5 label-font color-grey">
            Speakers Will be in this status once a nomination request has been submitted
          </p>
        </li>
        <li>
          <img src="../../assets/check.svg" alt="checks" />
          <span class="ms-4 color-green">PR Review</span>
          <p class="ms-5 label-font color-grey">
            Mostly used if PR is still in discussion or if the DBDs were permitted to submit
            nominations.
          </p>
        </li>
        <li>
          <div class="circle text-center d-inline-block">3</div>
          <span class="ms-4">Pending Medical Approval</span>
          <p class="ms-5 label-font color-grey">1st Approver</p>
          <div class="ms-5">
            <button class="btn deny-btn">Deny</button>
            <button class="btn approve-btn">Approve</button>
          </div>
        </li>
      </ul>
    </div>
  </div>
</template>
<style scoped>
.card {
  border-radius: 16px;
}
.nomination-header {
  font-size: 20px;
}
.label-font {
  font-size: 12px;
}
.new-badge {
  border: 1px solid #e9a905;
  background-color: #faedcb;
  color: #e9a905;
  border-radius: 100px;
}
.nomination-ul-list {
  list-style-type: none;
}
ul {
  margin: 0;
  padding: 0;
}
.color-green {
  color: #0cba69;
}

.circle {
  border-radius: 100%;
  background-color: #e9a905;
  color: #fff;
  width: 25px;
}

.deny-btn {
  border: 1px solid #0047cf;
  color: #0047cf;
  border-radius: 9px;
  width: 70px;
  height: 30px;
  font-size: 12px;
}

.approve-btn {
  background: #0047cf;
  color: #fff;
  border-radius: 9px;
  width: 80px;
  height: 30px;
  font-size: 12px;
  margin-left: 15px;
}
</style>
