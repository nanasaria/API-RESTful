<h1 align="center"> API-RESTFul </h1>
<h1>O que é uma API?</h1>
<p>
  <blockquote> Interface de Programação de Aplicativos - É um conjunto de rotinas e padrões de programação para acesso a um aplicativo de software. </blockquote>
</p>
<img src="https://hermes.dio.me/articles/cover/a30a16f5-8a78-4b6b-9b3c-a17b223c400d.png" height="300" />
  <br><i>Image: https://www.dio.me/articles/o-que-e-uma-api-Y8U6UW</i>
<br>
<h2>RESOURCE - Recursos são elementos que podem ser manipulados através de um ID.</h2>
<blockquote>A nomeação de um recurso é sempre um SUBSTANTIVO - Exemplo: Usuário.</p></blockquote>
<h2>URI - O que é?</h2>
<blockquote><p>Uniform Resource Identifier - Identificador uniforme de recursos é uma cadeia de caracteres usada para identificar ou denominar um recurso na internet.<br>
Uri: www.site.com/user</blockquote>
</p>
<h2>URL - O que é?  </h2>
<blockquote><p>Uniform Resource Locator - Localizador Padrão de Recursos é o endereço de um recurso disponível em uma rede.<br>
Exemplo: recurso: impressora. <br>
URL/URI: http://www.site.com/print. <br> 
URL vem acompanhada de um http. Ou seja, é o endereço completo.</p></blockquote>
<h2>URN - O que é?  </h2>
<blockquote><p>Uniform Resource Name - Nome Uniforme de Recurso é um tipo de URI que usa o URN Scheme e o objetivo é a identificação única do recurso de forma persistente e independente de sua localização. <br></blockquote>
<h2>IRI - O que é?</h2>
<blockquote><p>Internationalized Resource Identifier - Identificador de Recursos Internacionalizado é uma generalização do URI. Podendo conter caracteres do Conjunto Universal de caracteres.</p></blockquote>
<h1>O que é REST?</h1>
<blockquote><i>“No início dos anos 2000 Roy Fielding apresentou em sua tese de doutorado o padrão REST, o principal objetivo desse padrão era tentar resolver problemas do protocolo SOAP, como alta complexidade de implementação e lentidão na comunicação. “ - Rivaldo Junior. Modelo de maturidade de Richardson para APIs REST. MEDIUM, 1, setembro de 2020. Disponível em: https://rivaildojunior.medium.com/modelo-de-maturidade-de-richardson-para-apis-rest-8845f93b288.</i><br>
<br>REST - Representational State Transfer - Transferencia de estado representacional.
Foi criado para utilizar o protocolo HTTP e o URI de forma “correta”.</blockquote>
<img src="https://raw.githubusercontent.com/Codecademy/articles/0b631b51723fbb3cc652ef5f009082aa71916e63/images/rest_api.svg" height="350" />
<br><i>Image: https://www.dio.me/articles/o-que-e-uma-api-Y8U6UW](https://www.codecademy.com/article/what-is-rest</i>
<h1>CONTRAINS</h1>
<blockquote>
<b>Cliente - Servidor -> Separar as responsabilidades de de diferentes partes de um sistema. Permite escalar o back-end sem que mexa no front-end.</b><br><br>
<b>Stateless -> Propõe que cada requisição ao servidor não deve ter ligação com requisições anteriores ou futuras.</b><br><br>
<b>Cache -> Sistema REST deve permitir que suas respostas sejam passíveis de cache.</b><br><br>
<b>Interface Uniforme -> Possuir uma interface modelada seguindo padrões importantes.</b>
<ul>
<li>Recursos</li>
<li>Mensagens autodescritivas</li>
<li>Hypermedia</li>
</ul>
<br>
<b>Sistema em Camadas -> Sistema REST deve ter a capacidade de adicionar elementos intermediários e que sejam totalmente transparentes para seus clientes.</b><br><br>
<b>Código sob demanda -> Aumentar a flexibilidade dos clientes. Envia um código executável de um server a um cliente mediante solicitação do cliente. Essa prática reduz a visibilidade. Essa prática é opcional para o REST.</b><br><br></blockquote>

<h2>REST vs RESTful</h2>
<blockquote>
<b>REST</b> é a discussão sobre o modelo e as características REST. REST é um conjunto de melhorias práticas (CONSTRAINS).
<b>RESTful</b> é o uso dessas características REST. Ou seja, se uma API segue os princípios REST, ela é uma API RESTful.
  <br><b><i>Algumas representações são o XML e o JSON.</i></b>
</blockquote>

<h2>REST vs SOAP</h2>
<blockquote>
<b>SOAP</b> - Simple Object Access Protocol.
<br><b>REST</b> é um modelo arquitetural e o SOAP é um protocolo.
<br>
  <p><b>REST</p>
  <ul>
    <li>Modelo Arquitetural</li>
    <li>Suporta requisições HTTP simples.</li>
    <li>Suporta vários formatos (XML, JSON, YAML)</li>
  </ul><br>
   <p><b>SOAP</p>
  <ul>
    <li>Protocolo</li>
    <li>SOAP envelopado no HTTP para chamadas RPC (Remote Procedure call).</li>
    <li>Suporta somente XML.</li>
  </ul>
</blockquote><br>

<h1>Métodos HTTP</h1>
<blockquote>
  <ul>
    <li>GET - Utilizado para obter um recurso. Não importa quantas vezes for executado, o resultado será sempre o mesmo. “Pegar um recurso”.</li>
    <li>POST - Utilized para a criação de um recurso a partir do uso de uma representação. </li>
    <li>PUT - Utilizado para atualizar um determinado recurso e envia todos os dados no recurso.</li>
    <li>DELETE - Utilizado para apagar um determinado recurso.</li>
    <li>HEAD - Muito parecido com o GET, a diferença é que o servidor não retorna o Body, apenas o cabeçalho.</li>
    <li>OPTIONS - É forma que o cliente possui de perguntar ao servidor quais os requisitos para um determinado recurso. A ideia dele é para saber quais métodos podem ser aplicados ao recurso ou qual URL permitida para se comunicar com o recurso.</li>
    <li>TRACE - Ecoa de volta a requisição recebida para que o cliente veja se houveram mudanças e adições feitas por outros servidores. Ou seja, vai até o servidor e volta para mostrar o que aconteceu em todo o percurso.</li>
    <li>CONNECT - Converte a requisição de conexão para um túnel TCP/IP transparente, usualmente para facilitar comunicação criptografia com SSL (HTTPS) através de um proxy HTTP não criptografado.</li>
    <li>PATCH - Faz modificações parciais nos recursos, ou seja, faz a alteração de valores específicos de um recurso, ao invés de enviar todos os dados novamente.
</li>   
  </ul>
</blockquote>

<h3>Safe Methods</h3>
<blockquote>Métodos considerados “salvos. Não realizam nenhum efeito entre cliente - servidor.
Safe Methods conhecidos: GET e HEAD.</blockquote>
<h3>Metodos Idempotentes</h3>
<blockquote>Idempotência é uma propriedade matemática. Ela explica que ao executar diversas vezes um resultado, ele permanece com o resultado da primeira execução.
Métodos Idempotentes conhecidos: GET, HEAD, PUT, DELETE, OPTIONS e TRACE.</blockquote>

<h1>MODELO DE MATURIDADE RICHARDSON</h1>
<blockquote>Este modelo foi criado com a finalidade de tornar a criação de uma API RESTful em algo mais fácil.<br>
<b>Níveis 0, 1 e 2 são fáceis de implementar, porém não são considerados RESTful.</b>
</blockquote>
<ol>
  <li>Nivel 0: POX.
  <p>
    Neste nível, as mensagens podem ser serializadas em formatos como XML, JSON e outros. O formato da mensagem não é um fator para declarar como um sistema REST.
  </p>
<table>
<thead>
<th>Verbo HTTP</th>
<th>URI</th>
<th>Ação</th>
</thead>
<tbody>
<tr>
	<td>GET</td>
	<td>/buscarCliente/1</td>
	<td>Visualizar</td>
</tr>
<tr>
	<td>POST </td>
	<td>/salvarCliente</td>
	<td>Criar</td>
</tr>
<tr>
	<td>POST</td>
	<td>alterarCliente/1</td>
	<td>Alterar</td>
</tr>
<tr>
	<td>GET/POST</td>
	<td>/deletarCliente/1</td>
	<td>Deletar</td>
</tr>
</tbody>
</table>
    <b>Nível 0 não usa o HTTP de forma correta.</b>
  </li>
  <br>
  <li>Nível 1: Recursos.
  <p>Neste nível passamos a usar recursos como forma de modelar e organizar API. Neste nível não é necessário conhecer a funcionalidade de cada método, apenas o recurso ao qual se tem acesso.</p>
  <table>
<thead>
<th>Verbo HTTP</th>
<th>URI</th>
<th>Ação</th>
</thead>
<tbody>
<tr>
	<td>GET</td>
	<td>/cliente/1</td>
	<td>Visualizar</td>
</tr>
<tr>
	<td>POST </td>
	<td>/cliente</td>
	<td>Criar</td>
</tr>
<tr>
	<td>PUT</td>
	<td>/cliente/1</td>
	<td>Alterar</td>
</tr>
<tr>
	<td>DELETE</td>
	<td>/cliente/1</td>
	<td>Deletar</td>
</tr>
</tbody>
  </table>
  </li>
  <br>
  <li>Nível 2: Verbos HTTP.
  <p>Nesse nível o HTTP deixa de exercer um papel apenas de transporte. Os verbos passam a ser utilizados com o propósito no qual foram criados.</p>
    <i>STATUS CODE HTTP:
https://developer.mozilla.org/en-US/docs/Web/HTTP/Status</i>
    <b>Nível 2 usa os verbos HTTP de forma correta.<b>
</li><br>
    <li>
      Nível 3: HATEOAS.
      <br>Hypermedia as the Engine of Application State
      <br><br>Neste nível é implementado o hypermedia, que permite um documento descrever seu estado atual e quais os seus relacionamentos com outros futuros estados.
<br><br>Para entender melhor: https://deviniciative.wordpress.com/2020/11/12/entendendo-hypermedia-rest-apis-hateoas/
<br><br>Os formatos de resposta hipermídia geralmente agrupam links em um objeto JSON separado. Também é uma boa ideia usar um objeto JSON para representar um link. Isso nos dá a opção de adicionar mais informações aos links posteriormente.
<br>Exemplo: <link rel=“deletar” href=“/cliente/1” />
<br>Veja que o link rel está indicando o que será feito.
<br><br><b>No nível 3 temos controles de hipermídia!</b>
    </li>
</ol>
<br>
<h1>Media Types</h1>
<blockquote>
<p>Media Type é uma string que define qual o formato do dado e como ele deve ser lido pela máquina.
<br>Alguns Exemplos:</p>
<ul>
  <li>application/json</li>
  <li>application/xml</li>
  <li>multipart/form-data</li>
  <li>text/html</li>
</ul>
  <p>A primeira parte (antes da / ) pode conter um tipo registrado de alto nível, como:</p>
  <ul>
  <li>application</li>
  <li>audio</li>
  <li>example</li>
  <li>image</li>
  <li>message</li>
  <li>model</li>
  <li>multipart</li>
  <li>text</li>
  <li>video</li>
</ul>
</blockquote>
<h3>Media Type vs MIME Type</h3>
<blockquote>
  MIME Type: https://developer.mozilla.org/en-US/docs/Web/HTTP/Basics_of_HTTP/MIME_types/Common_types 
<br>As duas são a mesma coisa.
</blockquote>

<h1>ERROS</h1>
<blockquote>
  1xx Informacional: Códigos começados com 1 são conhecidos como códigos informais.
<br>2xx Success: Sucesso no intercâmbio entre servidor e cliente.
<br>3xx Redirection: Os códigos 3xx indicam que cliente deve fazer uma ação adicional antes da requisição estar completa.
<br>4xx Client Error: Existe algo errado com a requisição do cliente.
<br>5xx Server Error: O cliente enviou uma requisição válida, mas o servidor não processou com sucesso.
  <br><br>O ideal é sempre retornar o status code menos genérico e se necessário, uma message-body com detalhes do ocorrido.
</blockquote>

<h1>VERSIONAMENTO EM APIs</h1>
<blockquote>
<ol>
  <li>Subdomínio: api1.example.com/users</li>
  <li>URL: example.com/v1/users</li>
  <li>URL com parâmetros: example.com/users?v=1</li>
  <li>HTTP Header customizada: X-API-Version: 1</li>
  <li>Accept Header com Media Type customizado: Accept: application/vnd.myapi.v1+json</li>
  <li>Accept Header com opção de versão: Accept: application/vnd.myapi+json;version=1.0</li>
</ol>
  <br><br>Atualmente a mais utilizada é o versionamento através de URL, por ser fácil, evitar erros e permitir compartilhar facilmente.
</blockquote>

<h1>Caching</h1>
<blockquote>
  É extremamente importante para a redução de custos.
<br>As únicas coisas que NÃO devem ser cacheadas são as que mudam com muita frequência.
<br>Uma forma de checar se um cache está desatualizado é o processo de cache invalidation.
<br>O processo de cache invalidation: https://redis.io/glossary/cache-invalidation/
</blockquote>
<h3>O HTTP CONTA COM TUDO O QUE É NECESSÁRIO PARA FAZER UM CACHE DO LADO DO CLIENTE.</h3>
<blockquote>
  <ul>
    <li>Cache pode salvar uma enorme quantidade de tempo.</li>
    <li>A medida em que se diminui o tempo de requisição, as aplicações precisam de menos tempo para rodar, ou seja, gasta-se menos com servidor.</li>
    <li>Cache permite que uma aplicação escale mais facilmente.
</li>
  </ul>
</blockquote>

<h1>Cache no Cliente</h1>
<p>
Os objetivos do caching HTTP são eliminar o envio de requisições o máximo possível.
<br>O objetivo de reduzir pode ser alcançado com: Mecanismo de expiração Cache-Control e mecanismo de validação ETag ou Last Modified.
<br><br>Mínimo de requisições: Cache-Control.
<br>Mínimo de dados nas respostas: ETag.
<br><br>A maneira mais rápida de fazer uma requisição é não envia-la inteira e o header Cache-Control é usado para definir uma política de cache para um recurso.
</p>
<blockquote>
  Exemplo: 
<ul>
  <li>Cache-Control: max-age=3600</li>
  <li>Cache-Control: no-cache</li>
  <li>Cache-Control: private, max-age=86400</li>
</ul>
<br>
  Max-age especificamente em segundos quanto tempo o recurso pode ser cacheado.
<br>Private/public define quem pode fazer o cache. Public significa que qualquer um pode fazer o cache e o Private indica que apenas o browser pode fazer o cache.
<br><br>No-store informa que a resposta não deve ser armazenada no browser e nem em seus intermediários.
<br><br>No-cache significa que a resposta pode ser cacheada mas não pode ser recusada sem antes checar o servidor e ela pode ser combinada com um ETag.

<br><br>Mais sobre controle de cache: https://developer.mozilla.org/pt-BR/docs/Web/HTTP/Headers/
</blockquote>

<h1>ETag</h1>
<blockquote>
Entity Tag -> assegura um token de validação identificando uma versão especifica de uma resposta.
<br><br>ETag pode ser um HASH, mas o mais apropriado é o timestamp (data da última atualização) para verificar se o mesmo encontra-se desatualizado.
<br><br>Mais sobre: https://developer.mozilla.org/pt-BR/docs/Web/HTTP/Headers/ETag
</blockquote>

<h1>Autenticação</h1>
<p>Alguns sites podem gerenciar a autenticação através de cookies.
<br>Cookies são criados para permitir que o servidor grave e mantenha os estados (stateful), ou seja, uma requisição não depende da outra.</p>
<img src="https://www.oficinadanet.com.br/imagens/post/24811/o_que_sao_os_cookies_do_navegador.jpg" height="350"/>
<br><i>Image: https://www.oficinadanet.com.br/internet/24811-o-que-sao-os-cookies-do-navegador</i>
<br><br><blockquote>
  O padrão de esquema de autenticação HTTP basic é através de digest (baseado em uma contrain - Stateless).
<br><br>Quando uma aplicação web oferece ferramentas para outras aplicações, a autenticação pode ser feita através de uma API Key ou API secret token.
<br><br>Em resumo, uma API Key é uma combinação de letras e números, como um hash e fica sendo transmitida em todas as requisições para identificar aplicação. Geralmente é combinada de email e senha. Para garantir maior segurança, é importante que o servidor tenha configurado os certificados SSL.
</blockquote>

<h3>Identificação x Autenticação x Autorização</h3>
<blockquote>
<ul>
  <li><b>Identificação:</b> Usa-se apenas um identificador, uma API Key para serem identificados.</li>
  <li><b>Autenticação:</b> Usa-se um tipo de comprovação para autenticar quem é você. Por exemplo, e-mail e senha.</li>
  <li><b>Autorização:</b> Tem o intuito de definir o que você pode fazer de acordo com suas credenciais.</li>
</ul>
</blockquote>

<h3>Autenticação com HTTP</h3>
<blockquote>
  Os mecanismos padrões de autenticação com HTTP são definidos como basic e digest. Eles são relacionais ao contrain Stateless.
<br>Nesses mecanismos, o usuário e senha são incluídos em cada requisição codificados em Base64 para a autenticação Basic e com um hash MD5 para a autenticação Digest.
</blockquote>

<h3>Autenticação baseada em Token</h3>
<blockquote>
  Consiste em enviar o usuário/senha para o servidor e receber em troca um Token que será informado em cada requisição através da header Authorization.
<br><i>Diferenças entre stateful e stateless: https://www.redhat.com/pt-br/topics/cloud-native-apps/stateful-vs-stateless</i>
</blockquote>

<h3>Stateless Authentication</h3>
<blockquote>
<ul>
  <li><b>OAuth:</b> Protocolo aberto para permitir autorizações seguras em um método simples e padronizado.
  <br>Benefício do OAuth: Escalável.</li>
  <li><b>JWT:</b> É um padrão aberto para a transmissão segura entre partes como um objeto JSON e transmite essas informações de forma compacta e auto contida.</li>
</ul>
</blockquote>
