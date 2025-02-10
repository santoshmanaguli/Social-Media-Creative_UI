<script>
export default {
  data() {
    return {
      licenses: [
        {
          id: '1146-0452',
          state: 'State 1',
          country: 'Country 1',
          expiration_date: '10-16-2023',
          primary: true,
        },
        {
          id: '1146-0453',
          state: 'State 2',
          country: 'Country 2',
          expiration_date: '11-20-2024',
          primary: true,
        },
        {
          id: '1146-0454',
          state: 'State 3',
          country: 'Country 3',
          expiration_date: '12-15-2025',
          primary: true,
        },
      ],
    }
  },
}
</script>

<template>
  <div class="card">
    <div class="card-body">
      <div class="d-flex justify-content-between">
        <span class="card-title header-title color-blue font-weight500">Licenses </span>
        <img src="../assets/down_arrow.svg" alt="down arrow" />
      </div>
      <hr />
      <div class="d-flex justify-content-between align-items-center">
        <span> Click on add license and you can add more licenses here. </span>
        <button class="add-license-btn">
          <img src="../assets/plus_icon.svg" alt="" />
          <span class="ms-2">Add License</span>
        </button>
      </div>
      <br />
      <table class="table">
        <thead>
          <tr>
            <th class="p-4 table-headers" style="border-top-left-radius: 16px" scope="col">
              Action
            </th>
            <th class="p-4 table-headers" scope="col">
              License ID
              <img src="../assets/sort.svg" alt="" />
            </th>
            <th class="p-4 table-headers" scope="col">
              License State
              <img src="../assets/sort.svg" alt="" />
            </th>
            <th class="p-4 table-headers" scope="col">
              License Country
              <img src="../assets/sort.svg" alt="" />
            </th>
            <th class="p-4 table-headers" style="border-top-right-radius: 16px" scope="col">
              Expiration Date
              <img src="../assets/sort.svg" alt="" />
            </th>
          </tr>
        </thead>
        <tbody>
          <tr v-for="(license, index) in licenses" :key="index">
            <td>
              <img src="../assets/edit.svg" alt="" />
              &nbsp;
              <img src="../assets/delete.svg" alt="" />
            </td>
            <td>
              {{ license.id }}
              <span v-if="license.id === '1146-0452'" class="primary-yellow">Primary</span>
            </td>
            <td>{{ license.state }}</td>
            <td>{{ license.country }}</td>
            <td>{{ license.expiration_date }}</td>
          </tr>
        </tbody>
      </table>
    </div>
  </div>
</template>
<style scoped>
th {
  color: #6c757d;
  font-weight: 500;
  text-align: center;
}
td {
  text-align: center;
}
.card {
  border-radius: 16px;
}
.header-title {
  font-size: 20px;
}
.add-license-btn {
  border: 1px solid #0047cf;
  color: #0047cf;
  border-radius: 10px;
  padding: 8px;
  background: #fff;
}

.table-headers {
  background-color: #eff5ff;
}

.primary-yellow {
  background-color: #fff3cd;
  color: #ff8f0b;
  border-radius: 5px;
  padding: 2px 8px;
  font-size: 10px;
}
</style>
