<template>
    <div class = 'container'>
        <div class = 'row'>
            <div class = 'col-md-8'>
                <h2>Create an Account</h2>
                <form @submit.prevent = 'registerUser'>
                    <div class = 'form-group'>
                        <label for = 'First Name'> First Name </label>
                        <input type = 'text' name = 'fname' id = 'fname' placeholder = 'Enter First Name' v-model = 'fname' class="form-control"/>
                        <label for = 'Middle Initial'> Middle Initial </label>
                        <input type = 'text' name = 'Mname' id = 'Mname' placeholder = 'Enter First Name' v-model = 'Mname' class="form-control"/>
                        <label for = 'Last Name'> Last Name </label>
                        <input type = 'text' name = 'lname' id = 'lname' placeholder = 'Enter First Name' v-model = 'lname' class="form-control"/>
                        
                        <label for = 'Address'> Address </label>
                        <input type = 'text' name = 'Address' id = 'Address' placeholder = 'Enter First Name' v-model = 'address' class="form-control"/>
                        
                        <label for = 'Birth Date'> Birthday </label>
                        <input type = 'text' name = 'DOB' id = 'DOB' placeholder = 'Enter First Name' v-model = 'DOB' class="form-control"/>

                        <label for = 'Email Address'> Email </label>
                        <input type = 'email' name = 'Email' id = 'Address' placeholder = 'Enter First Name' v-model = 'Email' class="form-control"/>

                        <label for = 'Username'> Username </label>
                        <input type = 'text' name = 'Uname' id = 'Uname' placeholder = 'Enter Username' v-model = 'Uname' class="form-control"/>                                                
                       
                        <label for = 'Password'> Password </label>
                        <input type = 'password' name = 'password' id = 'pword' placeholder = 'Enter Password' v-model = 'password' class="form-control"/>  
                        <br>
            
                        <button type = "button" class = "cancelbtn">Cancel</button>
                        <button type = "submit" class ="signupbtn">Sign Up</button>
                    </div>
                </form>
            </div>
        </div>
    </div>
</template>

<script>
//import axios from 'axios'
//import router from '../router'
export default {
	data () {
		return {
            fname:'',
            Mname:'',
            lname:'',
            address:'',
            DOB:'',
            email:'',
            uname:'',
            password:'',
        }
    },
    methods: {
        registerUser() {
            if (this.fname === '') {
                alert('Please enter your First Name.')
            }
        }
    }
}
</script>