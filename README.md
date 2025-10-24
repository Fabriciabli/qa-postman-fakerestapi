# 🧪 QA |  API Testing com Postman — FakeRESTApi

Projeto de testes de API REST desenvolvido durante meu aprendizado em **Postman**, com o objetivo de praticar e demonstrar habilidades de **automação de testes de API** e **validação de endpoints CRUD**.

---

Portfólio de **Fabrícia Fernandes**, com 💙

## 🖇️ Índice

- [Objetivo](#objetivo)
- [Estrutura de Testes](#estrutura-de-testes)
- [Ferramentas Utilizadas](#ferramentas-utilizadas)
- [Escopo dos Testes](#escopo-dos-testes)
- [Resultados](#resultados)
- [Aprendizados](#aprendizados)
- [Próximos Passos](#próximos-passos)
- [Documentação de Testes](#documentacao-de-testes)
- [Autora](#autora)

---

## 🎯 Objetivo

Explorar o ciclo completo de testes em uma **API REST** utilizando as ferramentas**Postman**, **Newman** e **Swagger**, com base na API pública **FakeRESTApi.Web V1 (Swagger)**.

O objetivo foi compreender e aplicar os principais tipos de validações em testes de API, como:

- ✅ Validação de Status Code
- ✅ Validação de Contrato (Schema)
- ✅ Validação de Body (Response)
- ✅ Validação de Estrutura e Dados
- ✅ Automatização de testes com o Newman

Durante o processo, foram testados os seguintes endpoints da API:

- `Activities`
- `Authors`
- `Books`
- `CoverPhotos`
- `Users`

---

## 🧩 Estrutura de Testes

- **GET All** → Validação de retorno de array e status code  
- **GET by ID** → Validação de objeto e contrato  
- **POST** → Criação de recurso e schema validation  
- **PUT** → Atualização e validação de campos modificados  
- **DELETE** → Exclusão e cenários negativos (id inexistente) 

---

## 🧰 Ferramentas Utilizadas

- [**Postman**](https://www.postman.com/) – criação e execução de requisições  
- [**Newman**](https://www.npmjs.com/package/newman) – execução automatizada e geração de relatórios  
- [**Swagger**](https://swagger.io/tools/swagger-ui/) – documentação e exploração dos endpoints da API  
- [**JSON Schema Converter**](https://www.liquid-technologies.com/online-json-to-schema-converter) – validação de contratos e respostas da API  
- [**JavaScript (Tests Tab)**](https://learning.postman.com/docs/writing-scripts/script-references/test-examples/) – criação de asserts e validações personalizadas  
- [**Chai (BDD)**](https://www.chaijs.com/api/bdd/) – uso de sintaxe expressiva para escrita de testes e validações no Postman  

---

## 🔍 Escopo dos Testes

Os testes foram desenvolvidos para validar o comportamento completo dos endpoints da API, abrangendo:

- **Métodos CRUD (Create, Read, Update e Delete)** – garantindo o funcionamento correto das operações principais da API  
- **Validação de Status Codes** – conferindo se cada requisição retorna o código HTTP esperado  
- **Verificação do Corpo da Resposta (Body)** – assegurando que o conteúdo retornado corresponde ao contrato definido  
- **Validação de Headers e Tempo de Resposta** – checando cabeçalhos importantes e o desempenho das requisições  
- **Uso de Variáveis de Ambiente** – facilitando a parametrização e reutilização dos testes  
- **Chaining de Requests** – encadeando chamadas para simular fluxos reais de uso da API

---

## 📊 Resultados

Relatórios gerados com o **Newman**:

- [Relatório PDF](./docs/postman-report.pdf)
- [Resumo JSON](./newman/test-summary.json)
- [Relatório HTML](./newman/newman-report.html)

---

## 📚 Aprendizados

- Configuração de ambientes no Postman
- Automação de execução de coleções
- Escrita de asserts em JavaScript
- Geração de relatórios com Newman
- Interpretação de respostas RESTful

---

## 🧠 Próximos Passos

- **Automatizar execuções com Newman e GitHub Actions:**  
  Integrar as coleções do Postman a um pipeline de CI/CD, permitindo que os testes sejam executados automaticamente a cada push no repositório.

- **Implementar validação dinâmica com JSON Schema:**  
  Garantir que as respostas da API mantenham a estrutura e os tipos de dados esperados, utilizando schemas para validação automatizada.

- **Adicionar autenticação via token (JWT):**  
  Aprimorar os testes com cenários autenticados, validando fluxos de login, autorização e controle de acesso.

- **Explorar automação de interface com Cypress:**  
  Expandir o escopo do portfólio para testes end-to-end, integrando a validação da API com testes funcionais de interface.

---

## 📄 Documentação de Testes

- **Postman:**

  - 🔹 [README](./README.md)
  - 🔹 [Documentos](./docs/postman-report.pdf)
  - 🔹 [Evidências](./evidence/)
  - 🔹 [Newman](./newman/)
  - 🔹 [Notes](./notes/)
  - 🔹 [Postman Collection](./postman-collection/)
  
---

## 👩‍💻 Autora
<a href="https://www.linkedin.com/in/fabriciafernandes/" target="_blank">
  <p align="center">
    <img src="./image/eu.png" alt="Imagem da autora" width="150"; style="border-radius: 8%"/>
    <br/>
    <strong>Fabrícia Fernandes - QA Analyst</strong>
  </p>
</a>


<p align="center">
  <a href="https://github.com/Fabriciabli" target="_blank">
    <img src="https://img.shields.io/badge/GitHub-000?logo=github&logoColor=white" alt="GitHub"/>
  </a>
  <a href="https://www.linkedin.com/in/fabriciafernandes/" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?logo=linkedin&logoColor=white" alt="LinkedIn"/>
  </a>
  <br/>
  <strong>✍️ Repositório em evolução contínua. Feedbacks e sugestões são bem-vindos!</strong>
</p>


