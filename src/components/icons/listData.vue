<template>
    <!-- ทำการกำหนด Props(เพื่อส่งข้อมูลจาก parent ไป child, คล้าย attribute) คือ name, salary  -->
    <div>
        <ul>
            <li v-for="(employee, index) in employees" :key="index">
                <Person :name="employee.name" :salary="employee.salary" />
            </li>
        </ul>
    </div>
</template>

<script>
import Person from './Person.vue';
export default {
    name: "listData",
    components: { Person },
    props: ["employees"],
};
</script>

<style></style>
