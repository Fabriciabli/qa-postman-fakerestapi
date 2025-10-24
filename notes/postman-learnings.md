# Aprendizados no Postman

Durante o estudo e a prática com o **Postman**, desenvolvi conhecimentos essenciais para o teste e análise de APIs REST.  
Esses aprendizados reforçaram tanto o entendimento técnico sobre requisições HTTP quanto as boas práticas de organização, automação e validação de respostas.

## Principais aprendizados

- **Diferença entre Params, Body e Headers:**  
  Compreendi o papel de cada elemento no ciclo de uma requisição —  
  *Params* para o envio de variáveis na URL, *Body* para o conteúdo principal da requisição (como JSON) e *Headers* para metadados e autenticação.

- **Criação e utilização de variáveis globais e de ambiente:**  
  Aprendi a configurar **variáveis globais**, que podem ser acessadas por qualquer coleção, e **variáveis de ambiente (Environment)**, que permitem alternar rapidamente entre diferentes contextos de execução (por exemplo, ambiente de **dev**, **homologação** ou **produção**).  
  Esse aprendizado facilitou a parametrização de dados como URLs base, tokens de autenticação e IDs dinâmicos, deixando os testes mais reutilizáveis e organizados.

- **Uso de variáveis de coleção:**  
  Explorei o uso de variáveis específicas de cada coleção para armazenar dados temporários e parâmetros usados em múltiplas requisições dentro do mesmo conjunto de testes.

- **Criação de scripts de teste em JavaScript:**  
  Dominei o uso do objeto `pm` (Postman API) para validar respostas, analisar payloads e registrar logs de execução.  
  
  Exemplo:  
  ```javascript
  pm.test("Status code é 200", function () {
      pm.response.to.have.status(200);
  });
