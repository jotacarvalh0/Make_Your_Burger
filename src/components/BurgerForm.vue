<template>
    <p>Componente de Mensagem</p>
    <div>
        <form id="burguer-form">
            <div class="input-container">
                <label for="name">Nome do cliente: </label>
                <input type="text" id="name" name="name" :="name" placeholder="Digite o seu nome">
            </div>
            <div class="input-container">
                <label for="bread">Escolha o pão: </label>
                <select name="bread" id="bread" :="bread">
                    <option value="">Selecione o seu pão</option>
                    <option value="integral">integral</option>
                </select>
            </div>
            <div class="input-container">
                <label for="meat">Escolha a carne: </label>
                <select name="meat" id="meat" :="meat">
                    <option value="">Selecione o tipo de carne</option>
                    <option value="maminha">Maminha</option>
                </select>
            </div>
            <div class="input-container">
                <label for="optional">Selecione os opcionais: </label>
                <div class="chackbox-container">
                    <input type="checkbox" name="optional" :="optional" value="salame">
                    <span>Salame</span>
                </div>
            </div>
            <div class="input-container">
                <input type="submit" class="submit-btn" value="Criar meu Burger!">
            </div>
        </form>
    </div>
</template>

<script>
export default {
    name: 'BurgerForm'
}
</script>

<style>

</style>