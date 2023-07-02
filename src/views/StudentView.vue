<template>
    <div>
        <div class="card">
            <div class="card-header">
                <h4>Students
                <RouterLink to="/student/add" class="btn btn-primary float-end">
                    Add Student
                </RouterLink>
            </h4>
            </div>
            <div class="card-body">
                <table class="table table-bordered">
                    <thead>
                        <tr>
                            <th>ID</th>
                            <th>Username</th>
                            <th>Password</th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr>

                        </tr>
                    </tbody>
                </table>
            </div>
        </div>
    </div>
    
  </template>

<script>

import axios from 'axios'

export default{
    name:'students',
    data(){
        return{
            students:[]
        }
    },
    mounted(){

        console.log('I am here')
    },
    methods:{
        getStudents(){
            axios.get().then(res =>{

            })
        }
    },
}
</script>