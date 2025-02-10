<template>
  <nav aria-label="breadcrumb" style="--bs-breadcrumb-divider: '>'">
    <ol class="breadcrumb">
      <img src="../../assets/back_arrow.svg" alt="back_arrow" />&nbsp;&nbsp;
      <li class="breadcrumb-item text-decoration-underline">Speaker</li>
      <li class="breadcrumb-item text-decoration-underline">Richard</li>
      <li class="breadcrumb-item" aria-current="page">
        <a class="text-decoration-none" style="color: #0047cf" href="#">Profile Summary</a>
      </li>
    </ol>
  </nav>
</template>

<script>
export default {
  name: 'Breadcrumb',
}
</script>

<style scoped>
.breadcrumb {
  padding: 20px 20px 0px 20px;
  margin-bottom: 0px;
  font-weight: 500;
}
</style>
