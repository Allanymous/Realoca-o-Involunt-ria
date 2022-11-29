<h1 align="center">Realocacao-Involuntaria</h1>
Projeto desenvolvido em Html, Css, Javascript e Bootstrap com finalidade de ensino e exemplos de funcionalidades das 4 linguagens de programação citadas anteriormente.

<h1>Descrição</h1>

 Site em desenvolvimento para mineradora fictícia com uma seção direcionada ao cadastro e login de funcionários e/ou clientes, fotos e textos explicativos e que auxiliam o cliente a conhecer melhor a empresa e suas ações no mercado.
 A proposta é a finalização do site podendo ser adicionado mais informações e funcionalidades que consiga captar mais clientes com uma interface simples, interativa e que possa ser lida suas informações sem dificuldade. Os funcionários autorizados poderão fazer login para ter acesso a administração de seus respectivos trabalhos e área para cadastro de funcionários com um formulário intuitivo e que forneça o máximo de dados para a empresa.
# Funcionalidades

Dentre as diversas funcionalidades essas são algumas delas:

Navbar com logo e seção de login e senha:

 
```
<a class="navbar-brand" href="#"><img id="imagem-habitare" src="images/habitare.png"></a>
 </div>
   <div id="navbar" class="navbar-collapse collapse">
     <form class="navbar-form navbar-right">
       <div class="form-group">
          <input type="text" placeholder="Login" class="form-control1">
            </div>
              <div class="form-group">
                <input type="password" placeholder="Senha" class="form-control">
                   </div>
                     <button class="btn btn-success" onclick="entrar()">Entrar</button>
                         <button class="btn btn-danger" onclick="cadastro()">Cadastre-se</button>                   
```   

Formulário para envio de informações do usúario para a empresa:


```
<script>
        /* Função Validar */
        function validar() {
          // pegando o valor do nome pelos names
          var nome = document.getElementById("nome");
          var sobrenome = document.getElementById("sobrenome");
          var email = document.getElementById("email");
          var senha = document.getElementById("senha");
          var telefone = document.getElementById("telefone");
          var cep = document.getElementById("cep");
          var sexo = document.getElementById("sexo");
          var newsletter = document.getElementById("newsletter").checked;

          // verificar se o nome está vazio
          if (nome.value == "") {
            alert("Nome não informado");

            // Deixa o input com o focus
            nome.focus();
            // retorna a função e não olha as outras linhas
            return;
          }
          if (sobrenome.value == "") {
            alert("Sobrenome não informado");
            sobrenome.focus();
            return;
          }
          if (email.value == "") {
            alert("E-mail não informado");
            email.focus();
            return;
          }
          if (senha.value == "") {
            alert("Senha não informada");
            senha.focus();
            return;
          }
          if (telefone.value == "") {
            alert("Telefone não informado");
            telefone.focus();
            return;
          }
          if (cep.value == "") {
            alert("CEP não informado");
            cep.focus();
            return;
          }
          if (sexo.value == "") {
            alert("CEP não informado");
            sexo.focus();
            return;
          }
          alert("Formulário enviado!");
          // envia o formulário
          //formulario.submit();
        }
      </script>
```
