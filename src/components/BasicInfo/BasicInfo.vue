<template>
  <div class="d-flex">
    <div class="tabs d-flex gap-3 align-items-center">
      <span class="demo_selected">Demographics</span>
      <span>CV & Bio</span>
      <span>Preferences</span>
    </div>
    &nbsp; &nbsp;
    <div class="d-flex align-items-center">
      <div class="circle text-center">
        <img src="../../assets/protected.svg" alt="" />
      </div>
      &nbsp; &nbsp;
      <div class="circle1 text-center">
        <img src="../../assets/vector.svg" alt="" />
      </div>
    </div>
  </div>
  <br />
  <div class="card mb-3">
    <div class="card-body">
      <div class="d-flex justify-content-between">
        <span class="card-title color-blue font-weight500 header-title">Basic Information</span>
        <img src="../../assets/down_arrow.svg" alt="" />
      </div>
      <hr />
      <form>
        <div class="row g-3">
          <div class="col-md-4">
            <img src="../../assets/girl_photo.svg" alt="" />
          </div>
          <div class="col-md-4">
            <label for="firstName" class="form-label"
              ><img src="../../assets/edit.svg" alt=""
            /></label>
            <input type="text" class="form-control" id="firstName" placeholder="Ms." />
            <br />
            <label for="dob" class="form-label">
              <img src="../../assets/edit.svg" alt="" />&nbsp;
              <img src="../../assets/edit.svg" alt="" />
            </label>
            <input type="text" class="form-control" id="dob" placeholder="Nora" />
            <br />
            <label for="dob" class="form-label"> Pronouns </label>
            <input type="text" class="form-control" id="dob" placeholder="Nora" />
            <br />
            <label for="dob" class="form-label">
              <img src="../../assets/edit.svg" alt="" />
            </label>
            <input type="text" class="form-control" id="dob" placeholder="Noe" />
          </div>
          <div class="col-md-4">
            <label for="lastName" class="form-label">
              <img src="../../assets/edit.svg" alt="" />&nbsp;
              <img src="../../assets/edit.svg" alt="" />
            </label>
            <input type="text" class="form-control" id="lastName" placeholder="Doe" />
            <br />
            <label for="dob" class="form-label">
              <img src="../../assets/edit.svg" alt="" />
            </label>
            <input type="text" class="form-control" id="dob" placeholder="Noe" />
            <br />
            <label for="dob" class="form-label"> Date of Birth </label>
            <input type="date" class="form-control" id="dob" placeholder="Select Date" />
            <br />
            <label for="dob" class="form-label">
              <img src="../../assets/edit.svg" alt="" />
            </label>
            <input type="text" class="form-control" id="dob" placeholder="Noe" />
          </div>
        </div>
        <br />
        <div class="row justify-content-between">
          <div class="col-md-4">
            <label for="speaker"> Speaker Type </label>
            <input type="text" class="form-control" />
          </div>
          <div class="col-md-4">
            <label for="degree"> Degree </label>
            <input type="text" class="form-control" />
          </div>
          <div class="col-md-4">
            <label for="credential"> Credential(s) </label>
            <input type="text" class="form-control" />
          </div>
        </div>
        <br />
        <div class="row justify-content-between">
          <div class="col-md-4">
            <label for="speaker"> NPI# </label>
            <input type="text" class="form-control" />
          </div>
          <div class="col-md-4">
            <label for="degree"> Federal Employee </label>
            <div class="form-check form-switch">
              <input class="form-check-input" type="checkbox" id="federalEmployee" checked />
            </div>
          </div>
          <div class="col-md-4">
            <label for="degree"> Govt Employee </label>
            <div class="form-check form-switch">
              <input class="form-check-input" type="checkbox" id="federalEmployee" checked />
            </div>
          </div>
        </div>
      </form>
    </div>
  </div>
</template>
<style scoped>
.tabs {
  background-color: #fff;
  border-radius: 12px;
  max-width: fit-content;
  padding-right: 10px;
}

.demo_selected {
  border-radius: 12px;
  border: 2px solid #0047cf;
  color: #0047cf;
  padding: 8px;
  font-weight: 500;
}

.circle {
  border-radius: 100%;
  background-color: #ffd5b1;
  border: 1px solid #e76b03;
  width: 27px;
  height: 28px;
}

.circle1 {
  border: 1px solid #efa11f;
  background-color: #fff3cd;
  border-radius: 100%;
  width: 27px;
  height: 28px;
}

.header-title {
  font-size: 20px;
}

.form-check-input {
  width: 2.5rem;
  height: 1.5rem;
  background-color: #fff;
  border-radius: 1rem;
  transition: background-color 0.2s;
}
.form-check-input:checked {
  background-color: #0cba69;
  border-color: #0cba69;
}
.form-check-input:not(:checked) {
  background-color: #fff; /* White when unchecked */
  border-color: #ccc;
}
</style>
