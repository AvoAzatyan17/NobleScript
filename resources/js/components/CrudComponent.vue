<template>
    <div class="table-div">
        <h3 class="text-center">Crud list table</h3>
        <b-link href="#">Add new</b-link>
        <table class="table">
            <thead>
            <tr>
                <th>Value</th>
                <th>Edit</th>
                <th>Delete</th>
            </tr>
            </thead>
            <tbody>
            <tr>
                <td>
                    <b-form-input  placeholder="Enter value" @keyup="queryForKeywords"></b-form-input>
                </td>
                <td>
                    <b-link id="myDiv" ref="myDiv">{{ name }}</b-link>
                </td>
                <td>
                    <b-link href="#">Delete</b-link>
                </td>
            </tr>
            <tr>
                <td>
                    <b-form-input  placeholder="Enter value" @keyup="queryForKeywords"></b-form-input>
                </td>
                <td>
                    <b-link id="myDiv" ref="myDiv">{{ name }}</b-link>
                </td>
                <td>
                    <b-link href="#">Delete</b-link>
                </td>
            </tr>
            <tr>
                <td>
                    <b-form-input  placeholder="Enter value" @keyup="queryForKeywords"></b-form-input>
                </td>
                <td>
                    <b-link id="myDiv" ref="myDiv">{{ name }}</b-link>
                </td>
                <td>
                    <b-link href="#">Delete</b-link>
                </td>
            </tr>
            </tbody>
        </table>
    </div>
</template>
<script>
export default {
    data() {
        return {
            name: 'Edit',
        }
    },
    methods: {
        queryForKeywords(event) {
            const value = event.target.value
            this.keywords = value
            this.$refs.myDiv.$el.innerHTML = 'Change';
        }
    }
}
</script>

<style scoped>

</style>
