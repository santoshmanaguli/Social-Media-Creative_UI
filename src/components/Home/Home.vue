<template>
  <div class="container-fluid py-3">
    <div class="row">
      <!-- Sidebar -->
      <div class="col-md-3 col-12 mb-3">
        <MenuItems />
        <NominationStatus />
      </div>
      <!-- Main Content -->
      <div class="col-md-9 col-12">
        <BasicInfo />
        <Licenses />
      </div>
      <div class="row justify-content-end" style="margin-top: 10px">
        <button class="clear-btn">Clear</button>
        <button class="update-btn">Update All</button>
      </div>
    </div>
  </div>
</template>

<script>
import MenuItems from '@/components/MenuItems/MenuItems.vue'
import NominationStatus from '@/components/NominationStatus/NominationStatus.vue'
import BasicInfo from '../BasicInfo/BasicInfo.vue'
import Licenses from '../Licenses.vue'

export default {
  name: 'ProfileSummary',
  components: {
    MenuItems,
    NominationStatus,
    BasicInfo,
    Licenses,
  },
}
</script>

<style>
.card {
  border-radius: 10px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

.clear-btn {
  border-radius: 8px;
  background: #cacfd3;
  border: 1px solid #cacfd3;
  color: #424242;
  width: 7%;
  padding: 7px;
}

.update-btn {
  border-radius: 8px;
  background: #0047cf;
  border: 1px solid #0047cf;
  color: #fff;
  width: 10%;
  padding: 7px;
  margin-left: 10px;
}
</style>
