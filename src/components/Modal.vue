<template>
    <div class='modal'>
        <div>
            <p>Fale Conosco</p>
        </div>
        <p>Fale Conosco, estamos á disposição apra atendê-los!</p>
        <label>Nome: <input type="text" name="Name" > </label>
        <label>Email: <input type="text" name="Name" > </label>
        <label>Telefone(s): <input type="text" name="Name" > </label>
        <label>Mensagem: <textarea name="Mensagem"></textarea> </label>
    </div>
</template>


<style lang="scss">
.modal{
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    align-content: space-between;
    width: 50%;
    input , textarea{
        outline: none;
        border: 0 solid;

    }
}
</style>
