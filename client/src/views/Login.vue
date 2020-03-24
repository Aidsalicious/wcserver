<template>
    <div class = 'container'>
        <div class = 'row'>
            <div class = 'col-md-8'>
                <h1>Log In</h1>
                <form @submit.prevent = 'registerUser'/>
                    <div class = 'form-single'>
                        <label for='Usernamae'> Username </label>
                        <input type = 'text' name = 'Uname' id = 'Uname' placeholder = 'Enter First Name' v-model = 'Uname' class="form-control"/>
                        <label for = 'Password'> Password </label>
                        <input type = 'password' name = 'password' id = 'pword' placeholder = 'Enter Password' v-model = 'password' class="form-control"/>  
                        <br>
            
                        <button type = "reset" class = "cancelbtn">Reset</button>
                        <button type = "submit" class ="signupbtn">Log In</button>
                    </div>
            </div>
        </div>
    </div>
</template>