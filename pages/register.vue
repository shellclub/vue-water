<template>
    <v-container>
        <v-layout column>
        <v-flex xs12 sm6><h1 class="headline"><v-icon>move_to_inbox</v-icon> ลงทะเบียน</h1></v-flex>
        <v-flex xs12 sm6><v-text-field v-model="user" label="ชื่อผู้ใช้"></v-text-field></v-flex>
        <v-flex>
            <v-container grid-list-xl>
            <v-layout>
                <v-flex xs12 sm6><v-text-field v-model="pass" type="password" label="รหัสผ่าน"></v-text-field></v-flex>
                <v-flex xs12 sm6><v-text-field v-model="pass" type="password2" label="รหัสผ่านอีกครั้ง"></v-text-field></v-flex>
            </v-layout>
            </v-container>
        </v-flex>       
        <v-flex xs12><v-btn @click="register" :loading="loading"   :disabled="loading"
      color="info"  @click.native=" loader = 'loading'"><v-icon>touch_app</v-icon> ลงทะเบียน</v-btn></v-flex>
        </v-layout>
    </v-container>
</template>
<script>
export default {
    data(){
        return{
            user: '',
            pass: '',
            pass2: '',
        }
       },
        methods: {
        register() {
      },
   }
}
</script>

