<template>
  <div id="app">
    <navigation-bar/>
    <first-block id="section-one"/>
    <second-block id="section-two"/>
    <third-block id="section-three"/> 
    <fourth-block id="section-four"/>
    <home/>           
  </div>
</template>

<script>
import FirstBlock from '@/components/FirstBlock.vue'
import SecondBlock from '@/components/SecondBlock.vue'
import ThirdBlock from '@/components/ThirdBlock.vue'
import FourthBlock from '@/components/FourthBlock.vue'
import Home from '@/components/Home.vue'
import NavigationBar from '@/components/NavigationBar.vue'

  export default {
    name: 'app',
    components: {         
      FirstBlock,
      SecondBlock, 
      ThirdBlock,   
      FourthBlock,
      Home,
      NavigationBar,
    },
    data() {
      return {
        employees: [
          {
            id: 1,
            name: 'Richard Hendricks',
            email: 'richard@piedpiper.com',
          },
          {
            id: 2,
            name: 'Bertram Gilfoyle',
            email: 'gilfoyle@piedpiper.com',
          },
          {
            id: 3,
            name: 'Dinesh Chugtai',
            email: 'dinesh@piedpiper.com',
          },
        ],
      }
    },
    methods:{
      addEmployee(employee){
        const lastId = this.employees.length > 0 ? this.employees[this.employees.length - 1].id : 0;
        const id = lastId + 1;
        const newEmployee = { ...employee, id };
        this.employees = [...this.employees, newEmployee];
      },
      deleteEmployee(id){
        this.employees = this.employees.filter(
          employee => employee.id !== id
        )
      },
      editEmployee(id, updatedEmployee) {
        this.employees = this.employees.map(employee =>
          employee.id === id ? updatedEmployee : employee
        )
      }
    }
  }
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;  
  text-align: center;
  color: #2c3e50; 
}
</style>
