# Painel-Orcamentario
Relatório Power BI de monitoramento de orcamento com acesso dos dados enviados por email pelo T.G. da STN

Este projeto contém o arquivo Power BI e o código M do editor avançado para leitura das 3 planilhas enviadas pelo Serpro que são geradas pelo Tesouro Gerencial da Secretaria de Tesouro Nacional. Você pode usar os produtos sem licença da Microsoft Power BI Desktop e usar o Serviço Online do Office 360 para publicar o painel público sem custo.

Seu órgão precisa ter conta na STN e assinar o serviço de subscrição de e-mails do Tesouro Gerencial (não é escopo deste projeto como fazer isto).

Procure gerar 3 planilhas: Dotação Orçamentária, Despesas Obrigatórias e Despesas Discricionárias. Os dados principais podem ser vistos pelo Power Query do Painel.

O extrator irá ler cada planilha de uma pasta que vc deve criar na caixa do seu setor em seu órgão. Deverá ser criada uma regra no Outlook para filtrar o remetente “naoresponda@serpro.gov.br” e cujo assunto contenha os termos “dotação” ou “despesas”, movendo para esta subpasta (no exemplo,  subpasta TG_Orcamento). A fonte do ETL terá que ser alterada substituindo setor e orgão para o seu caso particular.

A estrutura da planilha poderá ter leves alterações comparadas com a utilizada neste painel (cabeçalho, linhas em branco) e o ETL do Power Query precisará ser editado para correção do formato da planilha que visa tabular os dados, retirando sub-totais e outras linhas desnecessárias.

Agende a carga do Painel no Serviço Online conforme sua escolha de subscrição do T.G. (1 dia da semana, Segundas e Sextas, etc.).

Faça bom uso!
