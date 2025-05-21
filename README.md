<h3 align="center">
  Desafio Front-End SR
</h3>

<h3 align="center">
  <img alt="Magento" 
    src="https://logosandtypes.com/wp-content/uploads/2020/07/magento.svg" width="180px"/>
</h3>

<hr/>

## Sobre o Desafio 🚀

### Customização do Checkout com integração a API externa (GET + POST)

Neste desafio, seu objetivo será customizar o **checkout do Magento 2**, utilizando o fallback do `Magento_Checkout`, criando **um componente Knockout.js** que consuma uma API externa com dados adicionais do cliente ou do pedido, e que envie um POST com informações no momento da finalização do pedido.

Imagine que o cliente do e-commerce quer **integrar o checkout com uma solução externa de antifraude**, ou **registrar a tentativa de pedido em outro sistema**.

---

### O que deve ser feito 🧩

1. Criar um **componente Knockout.js**, adicionado via layout XML, que:
   - Consulte uma API pública ou mockada (GET), por exemplo, para obter dados do CEP, IP, clima, ou dados genéricos;
   - Exiba os dados em algum local do checkout (preferencialmente na etapa de pagamento ou antes da finalização);
   - Ao clicar em "Finalizar Pedido", envie um POST para uma API externa com os dados do carrinho, usuário, ou dados processados no seu componente.

2. Esse POST deve ocorrer de forma assíncrona **antes da criação final do pedido**, simulando a coleta de dados ou envio para um sistema de terceiros (mockar endpoint é permitido).

---

### Requisitos Técnicos 📌

- Utilizar o fallback de `Magento_Checkout` (`Magento_Checkout/js/view`).
- Knockout.js: observar boas práticas de bind, observables e performance.
- Layout XML para injetar o novo componente no passo de pagamento.
- Pode usar uma API pública como [ViaCEP](https://viacep.com.br), [IPify](https://www.ipify.org/), [JsonPlaceholder](https://jsonplaceholder.typicode.com/), ou criar um mock no [Mocky.io](https://mocky.io).
- Customizar o HTML exibido pelo componente, mantendo estilo compatível com o Magento 2 (Luma ou Blank).
- Adicionar algum controle visual de estado (loading, erro, etc).

---

### Critérios de Avaliação ✔️

- Compreensão e domínio do fallback do checkout.
- Correta manipulação de eventos de finalização de pedido (ex: interceptar `placeOrder` ou utilizar `beforePlaceOrder`).
- Tratamento correto das respostas da API.
- Boas práticas em Knockout.js e XML.
- Separação e modularização do código (HTML, JS e templates).
- Código limpo, legível, versionado com mensagens claras.

---

### O que você pode fazer para se destacar ⭐

- Utilizar injeção de dependências corretamente (ex: `quote`, `customerData`, etc).
- Aplicar validação visual no componente.
- Mostrar estados de carregamento e erro de forma elegante.
- Criar uma interface bonita e coerente com o Magento.
- Fazer um README explicando a lógica de integração e como rodar o teste.

---

### Entrega e Instruções 📦

- Crie um fork e uma branch com seu nome e sobrenome.
- Comite apenas os arquivos criados/modificados no módulo de checkout (ex: layout XML, JS, templates).
- Pode ser usado qualquer versão do Magento 2 (indique no README).
- Prazo sugerido: 2 dias úteis para entrega.

---

### Tecnologias e Conceitos Utilizados 🧪

- **Magento 2 (Checkout)**  
- **Knockout.js**  
- **JavaScript (ES6+)**  
- **Layout XML**  
- **Integração com API (fetch/AJAX)**  
- **Tratamento assíncrono de dados**  
- **Experiência do usuário no checkout**

</br>
**Boa Sorte!** 🤞
