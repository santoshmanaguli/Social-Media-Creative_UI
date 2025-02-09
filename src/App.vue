<script>
import Navbar from './components/Navbar/Navbar.vue'
import Breadcrumb from './components/Breadcrumb/Breadcrumb.vue'
import Home from './components/Home/Home.vue'

export default {
  components: {
    Navbar,
    Breadcrumb,
    Home,
  },
}
</script>
<template>
  <div>
    <Navbar />
    <Breadcrumb />
    <Home />
  </div>
</template>
<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@500&display=swap');
* {
  font-family: 'Poppins';
}
body {
  background-color: #f7f8fb;
}

.font-weight500 {
  font-weight: 500;
}

.bell-icon {
  width: 20px;
  height: 20px;
  color: #fff;
  border-radius: 50%;
}
</style>
