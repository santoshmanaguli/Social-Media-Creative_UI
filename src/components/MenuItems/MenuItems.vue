<script>
import profileSummary from '../../assets/profile_summary.svg'
import compliance from '../../assets/compliance.svg'
import eligibility from '../../assets/eligibility_criteria.svg'
import utilization from '../../assets/utilization.svg'
import paymentDetails from '../../assets/payment_details.svg'
import speakerPortal from '../../assets/speaker_portal.svg'
import productOrdering from '../../assets/product_ordering.svg'

export default {
  data() {
    return {
      menu_items: [
        { title: 'Profile Summary', icon: profileSummary },
        { title: 'Compliance', icon: compliance },
        { title: 'Eligibility Criteria', icon: eligibility },
        { title: 'Utilization', icon: utilization },
        { title: 'Payment Details', icon: paymentDetails },
        { title: 'Speaker Portal', icon: speakerPortal },
        { title: 'Product Ordering', icon: productOrdering },
      ],
    }
  },
}
</script>
<template>
  <div>
    <div class="card">
      <div class="card-body">
        <ul class="menu-items-list" style="list-style-type: none">
          <li
            class="menu-items-list-items d-flex justify-space-evenly p-3"
            v-for="itm of menu_items"
            :style="
              itm.title === 'Profile Summary'
                ? 'background-color: #E7EFFF; color: #0047CF; border-radius: 12px;'
                : ''
            "
          >
            <div v-if="itm.title === 'Profile Summary'" class="profile-blue-box"></div>
            <img class="ms-2 menu-item-img" :src="itm.icon" :alt="itm.title" />
            <span class="ms-4 menu-title-item">{{ itm.title }}</span>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>
<style scoped>
.card {
  border-radius: 24px;
}
.menu-items-list {
  padding: 0;
  margin: 0;
  list-style-type: none;
}
.menu-item-img {
  width: 20px;
}

.profile-blue-box {
  width: 10px;
  background: #0047cf;
  border-top-right-radius: 20px;
  border-bottom-right-radius: 20px;
  right: 15px;
  position: relative;
}
</style>
