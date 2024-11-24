**2. Como você armazenaria os dados? Crie uma estrutura de pastas capaz de armazenar as respostas da API. Ela deve permitir manipulação, verificações, buscas e pesquisas rápidas.**

Pressuponho que a organização já possua um Data Lake e utilize a Medallion Architecture, composta pelas camadas Raw Zone, Silver Zone e Gold Zone.	

A definição detalhada da estrutura deve levar em consideração a regra de negócios da empresa, mas supondo que haja uma rotina de carga diária, a organização das pastas pode ser baseada no nome do endpoint da API e na 		data da extração.

Para facilitar a identificação e categorização dos dados, cada setor pode ser 	separado, e o nome das pastas deve incluir o endpoint e a data correspondente 	à carga. A estrutura ficaria da seguinte forma:

		**datalake:**

		rawzone: 
		
                bi/getFicalInovoice_24/11/2024/data.json
                
                res/getGuestChecks_24/11/2024/data.json
                
                org/getChargeBack_24/11/2024/data.json
                
                trans/getTransactions_24/11/2024/data.json
                
                inv/getCashManagementDetails_24/11/2024/data.json
            
		silverzone:
		
		bi/getFicalInovoice_24/11/2024/data.json
                
                res/getGuestChecks_24/11/2024/data.json
                
                org/getChargeBack_24/11/2024/data.json
                
                trans/getTransactions_24/11/2024/data.json
                
                inv/getCashManagementDetails_24/11/2024/data.json

		goldzone:
		
		bi/getFicalInovoice_24/11/2024/data.json
                
                res/getGuestChecks_24/11/2024/data.json
                
                org/getChargeBack_24/11/2024/data.json
                
                trans/getTransactions_24/11/2024/data.json
                
                inv/getCashManagementDetails_24/11/2024/data.json
