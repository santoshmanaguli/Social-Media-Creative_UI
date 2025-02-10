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
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300..800;1,300..800&family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');

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

.color-blue {
  color: #0047cf;
}

.color-grey {
  color: #8f8d92;
}
</style>
