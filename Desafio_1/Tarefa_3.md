3. **Transcreva o JSON para tabelas SQL. A implementação deve fazer sentido para operações de restaurante.**   
   **Descreva a abordagem escolhida em detalhes. Justifique a escolha.**

   Primeiramente, utilizei uma ferramenta de visualização de JSON (jsonviewer) para obter uma compreensão mais clara e detalhada da estrutura do arquivo. 

   Essa ferramenta foi fundamental para identificar objetos, tipos de dados e os relacionamentos entre eles.

   Após essa análise inicial, desenvolvi o [Modelo Conceitual](https://lucid.app/lucidchart/b75e9a63-2784-42c5-a695-e118965c03be/edit?viewport_loc=774%2C1159%2C2920%2C1421%2C0_0&invitationId=inv_798d8a05-7313-4392-a161-a74cc496cae2) utilizando a ferramenta Lucidchart. 

   Durante esse processo, defini as entidades e seus respectivos atributos. Para entidades que não possuíam atributos claros no JSON fornecido, deduzi possíveis atributos com base no significado implícito dos nomes das entidades.

   Além disso, em casos de entidades com atributos categóricos, como discount, tenderMedia e errorCode, decidi criar entidades separadas para representar essas categorias.

   Essa escolha visou garantir a atomicidade dos dados, seguindo boas práticas de modelagem de banco de dados relacional e evitando redundâncias.

   Com o modelo conceitual finalizado, passei para o modelo físico, utilizando a ferramenta SGBD MS SQL Server. Criei o banco de dados como "CB_LAB" e criei as tabelas e os relacionamentos por meio de scripts SQL. 

   Durante essa etapa, defini as chaves primárias (PK), chaves estrangeiras (FK), tipos de dados e apliquei técnicas para otimização do banco.

   Por fim, realizei a inserção de dados nas tabelas a partir do próprio JSON fornecido, garantindo que os dados fossem organizados de forma eficiente e consultáveis no banco de dados.