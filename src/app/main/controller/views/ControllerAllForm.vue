<template>
  <div class="controllerAllFrom">
    <header-nav />
    <controller-side-nave />
    <dashboard-slot>
      <search-form :id="0"/>
      <div class="controllerFormsblock">
        <div class="controllerForm">
          <div class="controllerFormImg"><img src="../../../../assets/imgs/google-forms.png" alt=""></div>
          <div class="controllerFormTitle"><h4> Personal Form</h4></div>
          <div class="controllerFormsubandtime"><p class="totalFormSub">2 From Submission</p><p class="formDateCreate">Create on: Feb 4,2022 4:55am</p></div>
          <div class="controllerFormAction"><img src="../../../../assets/imgs/editdata.png" alt="edit"> <img src="../../../../assets/imgs/eye.png" alt="eye"><img src="../../../../assets/imgs/history.png" alt="history"><img src="../../../../assets/imgs/delete.png" alt="delete"></div>
        </div>
      </div>
    </dashboard-slot>
  </div>
</template>

<script>
import ControllerSideNave from "../../../shared/components/ControllerSideNave.vue";
import HeaderNav from "../../../shared/components/HeaderNav.vue";
import DashboardSlot from "../../../slots/DashboardSlot.vue";
import SearchForm from '../components/SearchForm.vue';
export default {
  components: { HeaderNav, ControllerSideNave, DashboardSlot, SearchForm },
};
</script>
<style scoped>
.controllerFormsblock {
    padding: 10px 70px;
}
.controllerFormAction img {
    background: #192a6b;
    margin: 0 5px;
    padding: 6px;
    width: 24px;
    border-radius: 6px;
}
.controllerForm {
    display: flex;
    align-items: center;
    border: 1px solid;
    border-radius: 7px;
    padding: 10px 17px;
}

.controllerForm > div {
    flex: 1;
}

.controllerFormImg img {
    width: 18px;
}
/* 
.controllerFormTitle {
    font-size: 1.4rem;
    color: #192a6b;
    font-weight: 600;
} */

.controllerForm 
 .controllerFormImg {
    flex: .2;
}

.controllerFormsubandtime p {
    margin-bottom: 0;
}

.controllerFormAction {
    justify-content: end;
    display: flex;
    align-items: center;
    opacity: 0;
}
.controllerForm .controllerFormsubandtime {
    flex: .6 !important;
    opacity: 0;
}
.controllerForm:hover > div{
  opacity: 1;
}
</style>