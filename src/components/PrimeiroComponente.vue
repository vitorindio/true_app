<template>
<div>
    <h1>vue vue!</h1>
    <p>meu nome é {{nome}} e trabalho como {{profissao}} </p>
</div>

</template>

<script>
export default {
    name:'PrimeiroComponente',
    data() {
        return {
            nome:"Vitor",
            profissao:"estagiário"
        }
    },
}

</script>