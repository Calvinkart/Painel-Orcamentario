# Painel Orçamentário
Relatório Power BI de monitoramento do orçamento com acesso aos dados enviados por email pelo T.G. da STN

Este projeto contém o arquivo Power BI e o código M do editor avançado para leitura das 3 planilhas enviadas pelo Serpro que são geradas pelo Tesouro Gerencial da Secretaria de Tesouro Nacional com exemplos na árvore de arquivos.
Você pode usar os produtos sem licença do Microsoft Power BI Desktop e usar o Serviço Online do Office 360 para publicar o painel público sem custo.

Seu órgão precisa ter conta na STN e assinar o serviço de subscrição de e-mails do Tesouro Gerencial (não é escopo deste projeto como fazer isto).

Procure gerar 3 planilhas: Dotação Orçamentária, Despesas Obrigatórias e Despesas Discricionárias. Os dados principais podem ser vistos no Power Query do Painel ou nas planilhas exemplo (originais).

O extrator irá ler cada planilha de uma pasta que vc deve criar na caixa de email do seu setor em seu órgão e tranforma-la no formato tabular,  retirando sub-totais e outras linhas desnecessárias, mas poderão ser necessárias leves alterações comparadas com as utilizadas neste painel (cabeçalho, linhas em branco). Use modelo padrão de outro órgão para gerar dados similares às planilhas exemplo. A fonte do ETL terá que ser alterada substituindo setor e orgão do endereço de e-mail para o seu caso particular.

Deverá ser criada uma regra no Outlook para filtrar o remetente “naoresponda@serpro.gov.br” e cujo assunto contenha os termos “dotação” ou “despesas”, movendo para esta subpasta (no exemplo, subpasta TG_Orcamento). 
Agende a carga do Painel no Serviço Online conforme sua escolha de subscrição do T.G. (1 dia da semana, Segundas e Sextas, etc.).

Faça bom uso!

Créditos:
- Os KPIs do Painel foram baseados no painel do curso de Power BI com dados orçamentários da ENAP
- A extração de planilhas dentro de emails do Outlook foi feita com base em dicas do canal https://www.youtube.com/@RonanVico
