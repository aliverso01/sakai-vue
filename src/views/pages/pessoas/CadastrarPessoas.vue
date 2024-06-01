import InputGroup from 'primevue/inputgroup';
import InputGroupAddon from 'primevue/inputgroupaddon';

<template>
    <div class="">
        <h1>Cadastrar Pessoas</h1>
        <form>

            <!-- Informações Pessoais -->
            <div class="p-fluid formgrid grid">

                <div class="md:col-5 col-12">
                    <label for="nome">Nome:</label>
                    <input type="text" id="nome" name="nome" class="p-inputtext p-component">
                </div>
                <div class="md:col-4 col-12">
                    <label for="apelido">Apelido:</label>
                    <input type="text" id="apelido" name="apelido" class="p-inputtext p-component">
                </div>
                <div class="md:col-3 col-12">
                    <label for="cpf_cnpj">CPF/CNPJ:</label>
                    <InputMask id="basic" v-model="value" mask="999.999.999-99" placeholder="000.000.000-00" />
                </div>
                <div class="md:col-2 col-12">
                    <label for="nascimento">Nascimento:</label>
                    <InputMask v-model="value" mask="99/99/9999" placeholder="00/00/0000" />
                </div>
                <div class="md:col-5 col-12">
                    <label for="email">Email:</label>
                    <input type="email" id="email" name="email" class="p-inputtext p-component">
                </div>
                <div class="md:col-2 col-12">
                    <label for="telefone">Telefone:</label>
                    <InputMask v-model="value" mask="(99) 99999-9999" placeholder="(XX) XXXXX-XXXX" />
                </div>
                <div class="md:col-3 col-12">
                    <label for="instagram">Instagram:</label>
                    <input type="text" id="instagram" name="instagram" class="p-inputtext p-component">
                </div>
                <div class="md:col-3 col-12">
                    <label for="sexo">Sexo:</label>
                    <select id="sexo" name="sexo" class="p-inputtext p-component">
                        <option value="masculino">Masculino</option>
                        <option value="feminino">Feminino</option>
                    </select>
                </div>
                <div class="md:col-9 col-12">
                    <label for="nome_mae">Nome da Mãe:</label>
                    <input type="text" id="nome_mae" name="nome_mae" class="p-inputtext p-component">
                </div>
            </div>
            <!-- Endereço -->
            <h2>Endereço</h2>
            <div class="p-fluid formgrid grid">
                <div class="md:col-2 col-12">
                    <label for="cep">CEP:</label>
                    <input type="text" id="cep" name="cep" class="p-inputtext p-component">
                </div>
                <div class="md:col-5 col-12">
                    <label for="rua">Rua:</label>
                    <input type="text" id="rua" name="rua" class="p-inputtext p-component">
                </div>
                <div class="md:col-1 col-12">
                    <label for="numero">Número:</label>
                    <input type="text" id="numero" name="numero" class="p-inputtext p-component">
                </div>
                <div class="md:col-4 col-12">
                    <label for="complemento">Complemento:</label>
                    <input type="text" id="complemento" name="complemento" class="p-inputtext p-component">
                </div>
                <div class="md:col-4 col-12">
                    <label for="bairro">Bairro:</label>
                    <input type="text" id="bairro" name="bairro" class="p-inputtext p-component">
                </div>
                <div class="md:col-4 col-12">
                    <label for="cidade">Cidade:</label>
                    <input type="text" id="cidade" name="cidade" class="p-inputtext p-component">
                </div>
                <div class="md:col-4 col-12">
                    <label for="estado">Estado:</label>
                    <input type="text" id="estado" name="estado" class="p-inputtext p-component">
                </div>
            </div>
            <h2>Informações Adicionais</h2>
            <div class="p-fluid formgrid grid">
                <!-- Informações Adicionais -->
                <div class="md:col-12 col-12">
                    <textarea id="informacoes_adicionais" name="informacoes_adicionais"
                        class="p-inputtext p-component"></textarea>
                </div>
            </div>

            <!-- Informações para Campanha -->
            <h2>Informações para Campanha</h2>

            <div class="p-fluid formgrid grid">
                <div class="md:col-4 col-12">
                    <label for="nome_candidato">Nome do Candidato:</label>
                    <input type="text" id="nome_candidato" name="nome_candidato" class="p-inputtext p-component">
                </div>
                <div class="md:col-4 col-12">
                    <label for="banner_image">Banner Image:</label>
                    <input type="file" id="banner_image" name="banner_image" class="p-inputtext p-component">
                </div>
                <div class="md:col-4 col-12">
                    <label for="link_banner">Link do Banner:</label>
                    <input type="text" id="link_banner" name="link_banner" class="p-inputtext p-component">
                </div>
                <div class="md:col-4 col-12">
                    <label for="tipo_eleitor">Tipo de Eleitor:</label>
                    <input type="text" id="tipo_eleitor" name="tipo_eleitor" class="p-inputtext p-component">
                </div>
                <div class="md:col-4 col-12">
                    <label for="regiao_lideranca">Região de Liderança:</label>
                    <input type="text" id="regiao_lideranca" name="regiao_lideranca" class="p-inputtext p-component">
                </div>
                <div class="md:col-4 col-12">
                    <label for="confirmacao_apoio">Confirmação de Apoio:</label>
                    <select id="sexo" name="sexo" class="p-inputtext p-component">
                        <option value="masculino">Confirmado</option>
                        <option value="feminino">Indeciso</option>
                        <option value="feminino">Não Apoia</option>
                    </select>
                </div>
            </div>
            <div class="md:col-12 col-12 text-right">
            <Button label="Cadastrar" 
                    icon="pi pi-check" 
                    iconPos="right" 
                    style="font-size: 20px"/>
        </div>
        </form>
    </div>

</template>