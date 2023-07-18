<template>
  <div>
    <FormComponent></FormComponent>
    <listData :employees="employees" />
    <!-- em ตัวแรกคือชื่อ prop ตัวหลังคือ data ใช้ : bind -->
  </div>
</template>

<script>
import FormComponent from './components/icons/FormComponent.vue';
import listData from './components/icons/listData.vue';
export default {
  name: "App",
  components: { listData, FormComponent },
  data() {
    return {
      employees: [
        { name: "B1", salary: 15000 },
        { name: "B2", salary: 20000 },
        { name: "B3", salary: 10000 }
      ]
    }
  }

}

</script>

<style></style>
