# Desafio Engenharia de Dados - Coco Bambu

Olá, candidato! Bem-vindo!  
Queremos conhecer um pouco mais sobre a sua forma de desenvolver aplicações e resolver problemas. Por isso, preparamos um pequeno desafio, conforme descrito a seguir:

## DESAFIO 1

### 1. [Descrição do Esquema JSON](https://github.com/Lucasbzrra/Desafio_Eng_de_Dados_Coco_Bambu/blob/main/Desafio_1/Tarefa_1.md)
Com base no exemplo fornecido, descreva o esquema JSON correspondente. O esquema deve refletir a estrutura dos dados e como eles estão organizados.

### 2. [Contexto Adicional](https://github.com/Lucasbzrra/Desafio_Eng_de_Dados_Coco_Bambu/blob/main/Desafio_1/Tarefa_2.sql)
No exemplo fornecido, o objeto `detailLines` contém um `menuItem`. Ele também pode conter instâncias de:
- `discount`
- `serviceCharge`
- `tenderMedia`
- `errorCode`

### Tarefa:
- Transcreva o JSON para **tabelas SQL**. A implementação deve fazer sentido para operações de restaurante, refletindo a forma como os dados são organizados e armazenados para uma análise eficiente.

### 3. [Descrição da Abordagem](https://github.com/Lucasbzrra/Desafio_Eng_de_Dados_Coco_Bambu/blob/main/Desafio_1/Tarefa_3.md)
Descreva a abordagem que você escolheu para resolver este desafio. Justifique a sua escolha de maneira detalhada, abordando como a estrutura de dados foi pensada para otimizar as operações do restaurante e a análise dos dados.

---

## DESAFIO 2

Nossa equipe de inteligência de negócios precisa analisar a receita de todas as lojas de uma rede de restaurantes. Essas informações podem ser obtidas por meio de **5 endpoints de API**.

| **Method** | **API/Endpoint**                | **Payload**                                                                 |
|------------|---------------------------------|-----------------------------------------------------------------------------|
| POST       | `/bi/getFiscalInvoice`          | `busDt: string(date)`, `storeId: string`                                    |
| POST       | `/res/getGuestChecks`           | `busDt: string(date)`, `storeId: string`                                    |
| POST       | `/org/getChargeBack`            | `busDt: string(date)`, `storeId: string`                                    |
| POST       | `/trans/getTransactions`        | `busDt: string(date)`, `storeId: string`                                    |
| POST       | `/inv/getCashManagementDetails` | `busDt: string(date)`, `storeId: string`                                    |

**Observação:**  
- `storeId` corresponde ao identificador da loja.  
- `busDt` corresponde à data de operação.

### 1. [Por que armazenar as respostas das APIs?](https://github.com/Lucasbzrra/Desafio_Eng_de_Dados_Coco_Bambu/blob/main/Desafio_2/Tarefa_1.md)
Explique as razões pelas quais é importante armazenar as respostas das APIs no data lake. Considere questões de desempenho, integridade dos dados e facilidade de análise.

### 2. [Como você armazenaria os dados?](https://github.com/Lucasbzrra/Desafio_Eng_de_Dados_Coco_Bambu/blob/main/Desafio_2/Tarefa_2.md)
Crie uma **estrutura de pastas** capaz de armazenar as respostas das APIs. A estrutura deve permitir manipulações eficientes, verificações rápidas e consultas de dados. Considere a escalabilidade e a facilidade de acesso aos dados.

### 3. [Alteração no Endpoint `getGuestChecks`](https://github.com/Lucasbzrra/Desafio_Eng_de_Dados_Coco_Bambu/blob/main/Desafio_2/Tarefa_3.md)
Considere que a resposta do endpoint `getGuestChecks` foi alterada, por exemplo, o campo `guestChecks.taxes` foi renomeado para `guestChecks.taxation`.  
Explique o impacto dessa alteração. O que isso implicaria no armazenamento e na manipulação dos dados?

---

### Observações Finais:
- O objetivo deste desafio é avaliar a sua capacidade de análise, organização de dados e a abordagem escolhida para resolver problemas de engenharia de dados em um ambiente real de restaurante.
- Pense em soluções que possam ser escaláveis e facilmente mantidas à medida que o volume de dados cresce.

Boa sorte!

### Documentação das Etapas com o Método Kanban ###

🔗 Confira os detalhes no seguinte link:   [KANBAN](https://trello.com/invite/b/67447bd4b8672da01ee4f6e0/ATTI9475017ca2ceac4735c5499130c2e84fAA5FDF6B/eng-dados)



### Estrutura do Projeto ###

```plaintext
├── Desafio_1/
│   ├── Tarefa_1.md
│   ├── Tarefa_2.md
│   └── Tarefa_3.md
|
├── Desafio_2/
│   ├── Tarefa_1.md
│   ├── Tarefa_2.md
│   └── Tarefa_3.md
│
└── README.md

