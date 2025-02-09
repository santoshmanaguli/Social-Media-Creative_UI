<script>
export default {
  name: 'Navbar',
  data() {
    return {
      nav_header: [
        { title: 'Program' },
        { title: 'Speaker' },
        { title: 'Venue' },
        { title: 'Report' },
        { title: 'Assignment Process' },
        { title: 'Reps' },
        { title: 'Console' },
        { title: 'Content' },
        { title: 'Task Management' },
      ],
      profile_info: {
        name: 'John Noe',
        position: 'Project Co-ordinator',
      },
    }
  },
}
</script>
<template>
  <nav class="navbar navbar-expand-lg navbar-light bg-light">
    <div class="container-fluid">
      <a class="navbar-brand logo-header" href="#">LOGO</a>
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarNav"
        aria-controls="navbarNav"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav me-auto">
          <div v-for="(nav, index) of nav_header" :key="index">
            <li class="d-flex align-items-center navbar-color" v-if="nav.title === 'Program'">
              <a class="nav-link" href="#">{{ nav.title }} </a>
              <i class="fa fa-angle-down" style="font-size: 16px; color: #424242"></i>
            </li>
            <li class="border-radius-blue" v-else-if="nav.title === 'Task Management'">
              <a class="nav-link" href="#">{{ nav.title }}</a>
            </li>
            <li v-else :style="nav.title === 'Speaker' ? 'color: #0047CF' : ''">
              <a
                class="nav-link"
                href="#"
                :style="nav.title === 'Speaker' ? 'color: #0047CF' : ''"
                >{{ nav.title }}</a
              >
            </li>
          </div>
        </ul>
        <div class="d-flex align-items-center gap-3">
          <div>
            <img src="../../../src/assets/filter.svg" alt="filter_icon" />
            <!-- <div class="bell-icon" style="background-color: #0047cf">1</div> -->
          </div>
          <div>
            <img src="../../../src/assets/bell_icon.svg" alt="bell_icon" />
          </div>
          <div>
            <img src="../../../src/assets/question_mark.svg" alt="question_mark" />
          </div>
          <div class="horizontal-line"></div>
          <div>
            <p class="mb-0 profile-name">{{ profile_info.name }}</p>
            <p class="mb-0 text-muted user-position">{{ profile_info.position }}</p>
          </div>
          <img
            src="../../assets/profile-photo.svg"
            alt="profile"
            class="rounded-circle"
            width="40"
          />
        </div>
      </div>
    </div>
  </nav>
</template>

<script></script>

<style scoped>
.navbar {
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  background-color: #ffffff !important;
}
.logo-header {
  color: #424242;
  font-size: 24px;
}
.border-radius-blue {
  border: 2px solid #0047cf;
  border-radius: 4px;
}
.profile-name {
  font-size: 14px;
  font-weight: 600;
}
.user-position {
  font-size: 12px;
  color: #8f8d92 !important;
}
.horizontal-line {
  height: 30px; /* Adjust the height */
  width: 2px;
  background-color: #cacfd3;
  margin: 0 10px;
}
</style>
