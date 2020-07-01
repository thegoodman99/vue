<template>
    <div>
        <form @submit.prevent="onSubmit($event)">
            <div class="form-group">
                <label for="user_name">Name</label>
                <input type="text" name="" id="user_name" v-model="user.name"/>
            </div>
            <div class="form-group">
                <label for="user_email">Name</label>
                <input type="email" name="" id="user_email" v-model="user.email"/>
            </div>
            <div class="form-group">
                <button type="submit">update</button>
            </div>
        </form>
    </div>
</template>
<script>
export default {
    data(){
        return {
            user: {
                id: null,
                name: "",
                email: ""
            }
        };
    },
    methods: {
        onsubmit(event){
            // @todo form submit event
        }
    },
    created() {
        // @todo load user details
    }
};
</script>
