# Entendimento da FakeRESTApi.Web V1

- **Base URL:** [`https://fakerestapi.azurewebsites.net/index.html`](https://fakerestapi.azurewebsites.net/index.html)

A **FakeRESTApi.Web V1** é uma API pública utilizada para fins educacionais e de prática em testes de APIs REST.  
Ela simula um ambiente real, disponibilizando endpoints que permitem executar operações completas de **CRUD** (*Create, Read, Update, Delete*) sobre diferentes recursos.

## Recursos testados

- `/Activities`
- `/Authors`
- `/Books`
- `/CoverPhotos`
- `/Users`

Cada um desses endpoints foi explorado individualmente, validando tanto o comportamento funcional quanto o retorno esperado em diferentes cenários.

Durante os testes:
- Foram criadas e manipuladas **massas de dados reais e fictícias** para validar as operações de leitura, criação, atualização e exclusão.
- Foram analisados **status codes**, **tempo de resposta**, **estrutura do payload** e **consistência dos dados**.
- Todos os testes foram realizados no **Postman**, com execução automatizada via **Newman** para geração de relatórios técnicos.

Essa análise teve como objetivo avaliar o comportamento geral da API, identificar eventuais falhas e compreender seu fluxo de comunicação REST de ponta a ponta.
