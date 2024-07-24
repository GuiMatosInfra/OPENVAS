<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Instalação do OpenVAS com Docker</title>
</head>
<body>
  <h1>Instalação do OpenVAS com Docker</h1>

  <h2>Passo 1: Instalação do Docker</h2>
  <pre>
    <code>sudo apt update</code><br>
    <code>sudo apt install docker.io</code>
  </pre>

  <h2>Passo 2: Executar o Contêiner Docker do OpenVAS</h2>
  <pre>
    <code>sudo docker run -d -p 443:443 --name openvas mikesplain/openvas</code>
  </pre>

  <p>Depois de executar este comando, o contêiner do OpenVAS estará em execução.</p>

  <h2>Verificação e Acesso ao OpenVAS</h2>
  <p>Para verificar se o contêiner está em execução e acessar a interface web:</p>
  <pre>
    <code>sudo docker ps</code>
  </pre>
  <p>Acesse a interface web do OpenVAS através de:</p>
  <pre>
    <code>https://localhost</code> ou <code>https://&lt;ip_do_seu_servidor&gt;</code>
  </pre>

  <p>Substitua <code>&lt;ip_do_seu_servidor&gt;</code> pelo endereço IP do seu servidor Debian.</p>

  <h3>Nota de Segurança</h3>
  <p>É importante configurar medidas de segurança adequadas antes de expor o OpenVAS publicamente.</p>

  <h3>Credenciais Padrão</h3>
  <p>Nome de usuário: <code>admin</code></p>
  <p>Senha: <code>admin</code></p>
</body>
</html>
