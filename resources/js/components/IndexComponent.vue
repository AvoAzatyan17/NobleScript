<template>
    <div>
        <div class="header-title">
            <h1>Noble Task</h1>
        </div>
        <b-card-group deck>
            <b-card header="CRUD" header-tag="header">
                <b-card-text>Make new crud action</b-card-text>
                    <b-button href="/crud" variant="primary">Go CRUD</b-button>
            </b-card>
            <b-card header="Tic Tac Toe" header-tag="header">
                <b-card-text>Go game page and play</b-card-text>
                <b-button href="/game" variant="success">Go Game</b-button>
            </b-card>
        </b-card-group>
    </div>
</template>

<script>
export default {
    mounted() {
        console.log('Component mounted.')
    }
}
</script>
