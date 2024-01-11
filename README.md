<!DOCTYPE html>
<!DOCTYPE HTML>
<html lang="Pt-br"> 
    <head> 
	     <title>Banco de Dados de Usuário</title>
		     <meta charset="UTF-8"/>
	</head>
	    <body> 
		    <div>
			    <form name="Bancos de Dados" method="POST" action="Resposta-Banc-Dados.php">		
			        <h1>Log in de Usuário</b></h1>
		            <p><input type="text" name="nome" placeholder="Nome de Usuário" required="required"/>
			        <p><input type="text" name="Matrícula" placeholder="Insira a Matrícula" required="required"/>
			        <p><input type="password" name="senha" placeholder="Insira sua senha" required="required"/>
            <style>
                  .password-container {
            position: relative;
            width: 250px;
        }
           .show-password-icon {
            position: absolute;
            right: 5px;
            top: 50%;
            transform: translateY(-50%);
            cursor: pointer;
        }
    </style>
                         <div class="password-container">
        <label for="senha">Senha:</label>
        <input type="password" id="senha" name="senha" placeholder="Insira sua senha" required="required" />
        <span class="show-password-icon" onclick="togglePasswordVisibility()">👁️</span>
    </div>
    <script>
        function togglePasswordVisibility() {
            const senhaInput = document.getElementById("senha");
            senhaInput.type = (senhaInput.type === "password") ? "text" : "password";
        }
    </script>
                    <p><input type="text" name="CPF" placeholder="Digite seu CPF" required="required"/>
			        <p><select name="Sexo">
		   	        <option value="">Sexo do Usuário</option>
		            <option value="masculino">Masculino</option>
				    <option value="feminino">Feminino</option>
			      </select>
		          </p>
			     <p><input type="submit" value="Enviar" /></p>
			</div>
		</body>
</html>
