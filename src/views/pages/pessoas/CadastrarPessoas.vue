<template>
    <div>
        <h1>Cadastrar Pessoas</h1>
        <form>

            <!-- Informações Pessoais -->
            <h2>Informações Pessoais</h2>
            <div class="p-fluid formgrid grid">
            <div>
                <label for="foto">Foto:</label>
                <input type="file" id="foto" name="foto" class="p-inputtext p-component">
            </div>
            <div>
                <label for="nome">Nome:</label>
                <input type="text" id="nome" name="nome" class="p-inputtext p-component">
            </div>
            <div>
                <label for="apelido">Apelido:</label>
                <input type="text" id="apelido" name="apelido" class="p-inputtext p-component">
            </div>
            <div>
                <label for="cpf_cnpj">CPF/CNPJ:</label>
                <input type="text" id="cpf_cnpj" name="cpf_cnpj" class="p-inputtext p-component">
            </div>
            <div>
                <label for="nascimento">Nascimento:</label>
                <input type="date" id="nascimento" name="nascimento" class="p-inputtext p-component">
            </div>
            <div>
                <label for="email">Email:</label>
                <input type="email" id="email" name="email" class="p-inputtext p-component">
            </div>
            <div>
                <label for="telefone">Telefone:</label>
                <input type="tel" id="telefone" name="telefone" class="p-inputtext p-component">
            </div>
            <div>
                <label for="instagram">Instagram:</label>
                <input type="text" id="instagram" name="instagram" class="p-inputtext p-component">
            </div>
            <div>
                <label for="sexo">Sexo:</label>
                <select id="sexo" name="sexo" class="p-inputtext p-component">
                    <option value="masculino">Masculino</option>
                    <option value="feminino">Feminino</option>
                </select>
            </div>
            <div>
                <label for="nome_mae">Nome da Mãe:</label>
                <input type="text" id="nome_mae" name="nome_mae" class="p-inputtext p-component">
            </div>
            </div>
            <!-- Endereço -->
            <h2>Endereço</h2>
            <div class="p-fluid formgrid grid">
            <div>
                <label for="cep">CEP:</label>
                <input type="text" id="cep" name="cep" class="p-inputtext p-component">
            </div>
            <div>
                <label for="rua">Rua:</label>
                <input type="text" id="rua" name="rua" class="p-inputtext p-component">
            </div>
            <div>
                <label for="numero">Número:</label>
                <input type="text" id="numero" name="numero" class="p-inputtext p-component">
            </div>
            <div>
                <label for="complemento">Complemento:</label>
                <input type="text" id="complemento" name="complemento" class="p-inputtext p-component">
            </div>
            <div>
                <label for="bairro">Bairro:</label>
                <input type="text" id="bairro" name="bairro" class="p-inputtext p-component">
            </div>
            <div>
                <label for="cidade">Cidade:</label>
                <input type="text" id="cidade" name="cidade" class="p-inputtext p-component">
            </div>
            <div>
                <label for="estado">Estado:</label>
                <input type="text" id="estado" name="estado" class="p-inputtext p-component">
            </div>
        </div>
            <div class="p-fluid formgrid grid"> 
            <!-- Informações Adicionais -->
            <h2>Informações Adicionais</h2>
            <div>
                <label for="informacoes_adicionais">Informações Adicionais:</label>
                <textarea id="informacoes_adicionais" name="informacoes_adicionais" class="p-inputtext p-component"></textarea>
            </div>
        </div>

            <!-- Informações para Campanha -->
            <h2>Informações para Campanha</h2>
            <div class="p-fluid formgrid grid">
            <div>
                <label for="nome_candidato">Nome do Candidato:</label>
                <input type="text" id="nome_candidato" name="nome_candidato" class="p-inputtext p-component">
            </div>
            <div>
                <label for="banner_image">Banner Image:</label>
                <input type="file" id="banner_image" name="banner_image" class="p-inputtext p-component">
            </div>
            <div>
                <label for="link_banner">Link do Banner:</label>
                <input type="text" id="link_banner" name="link_banner" class="p-inputtext p-component">
            </div>
            <div>
                <label for="tipo_eleitor">Tipo de Eleitor:</label>
                <input type="text" id="tipo_eleitor" name="tipo_eleitor" class="p-inputtext p-component">
            </div>
            <div>
                <label for="regiao_lideranca">Região de Liderança:</label>
                <input type="text" id="regiao_lideranca" name="regiao_lideranca" class="p-inputtext p-component">
            </div>
            <div>
                <label for="confirmacao_apoio">Confirmação de Apoio:</label>
                <input type="checkbox" id="confirmacao_apoio" name="confirmacao_apoio" class="p-inputtext p-component">
            </div>

            <button type="submit">Cadastrar</button>
        </div>
        
        </form>
    </div>
    
</template>