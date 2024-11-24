 1. Ao analisar o JSON fornecido, identifiquei que ele é um conjunto de dados estruturados que representa informações de comandas, incluindo impostos, itens 	consumidos, descontos, falhas e serviços.

	**guestChecks**:

	É um array que armazena os dados das comandas. Cada elemento contém informações detalhadas, como o ID da mesa, data e hora de início e fechamento, dados financeiros e aspectos logísticos relacionados à comanda.

	**taxes**:

	É um array presente dentro de cada objeto do guestChecks. Ele armazena informações sobre as taxas de imposto aplicáveis à comanda, incluindo valores e 	alíquotas.

	**detailLines**:

	É outro array dentro de guestChecks. Ele lista os itens consumidos, sendo que cada 	elemento do array representa um único produto, com detalhes específicos, como quantidade e valor.

	**menuItem**:

	É um objeto aninhado dentro de detailLines, que contém informações detalhadas sobre o produto consumido, como preços, níveis de preço e impostos aplicáveis.

	Além disso, o JSON também prevê a presença de quatro outros objetos que não foram incluídos neste exemplo:

	**discount**: Relacionado a descontos aplicáveis às comandas.

	**serviceCharge**: Representa serviços adicionais que podem ser incluídos.

	**tenderMedia**: Associado aos métodos de pagamento utilizados. Como este objeto não está presente no exemplo, deduzi sua função com base no nome.

	**errorCode**: Relacionado a erros que podem ocorrer durante o processamento dos dados.

	

	No link abaixo desenvolvi um dicionário de dados que representa o JSON fornecido.

	[Dicionario De Dados](https://docs.google.com/spreadsheets/d/1RCReMLE22gaI-pbuK4jm3s2uXuRrq9cETcGkmwsFMrY/edit?usp=sharing)
