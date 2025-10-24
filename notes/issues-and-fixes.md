# Problemas e Soluções

**Erro 400 em POST /Books**
- **Causa:** campo `id` enviado manualmente, mas o servidor gera automaticamente.
- **Solução:** remover o campo `id` do corpo da requisição.

---

**Falha no DELETE /Activities**
- **Causa:** requisição usando ID inexistente.
- **Solução:** criar um item antes de tentar deletar.

---

**Duração acima de 200ms em requisições da API**
- **Causa:** algumas rotas, como `GET /Books` e `GET /Authors`, apresentaram tempos de resposta acima de 200ms, possivelmente devido à latência do servidor de teste (FakeRESTApi) ou volume de dados retornado.
- **Impacto:** aumento no tempo total de execução da coleção e possível impacto na experiência do usuário final.
- **Solução/Análise:**
  - Verificar se a API é hospedada em ambiente gratuito (por exemplo, Azure WebApp com cold start).
  - Reexecutar os testes em horários diferentes para comparar desempenho.
  - Anotar tempos médios de resposta e definir limiares aceitáveis no Postman com scripts como:
    ```javascript
    pm.test("Tempo de resposta abaixo de 200ms", function () {
        pm.expect(pm.response.responseTime).to.be.below(200);
    });
    ```
  - Caso o tempo continue alto, incluir observação no relatório informando que a API de testes não está otimizada para desempenho.