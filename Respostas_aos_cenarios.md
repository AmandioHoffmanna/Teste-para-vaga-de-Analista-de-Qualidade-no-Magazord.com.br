**1° Cenário:**
1. Documentação e Materiais de Apoio:
  * Identificação da documentação: Seria utilizado para embasamento dos testes, a documentação disponível dos marketplaces do qual seria realizado a integração, revisando como ocorre a funcionalidade de suas API´s, revisando os requisitos funcionais e não funcionais do projeto, além das informações disponíveis pela equipe de regra de negócio, caso estiver disponível.
  * Análise da Documentação: Para realizar a análise da documentação, iria revisar os requisitos funcionais e não funcionais, correlacionando com a documentação disponível pelo marketplace e traçando um relacionamento entre eles.
  * Mapeamento dos requisitos: Iria relacionar cada requisito com uma cenário de teste específico para ele. Por exemplo; Caso um requisito seja, suportar grande volume de requisições simultâneas, atrás de ferramentas, iria simular esse cenário a fim de verificar se o requisito em questão está sendo atendido. 
  * Utilização de ferramentas: Se tratando especificamente de ferramentas, por não haver contato com as mesmas, pouco posso comentar a respeito. Entre as que tenho mais conhecimento, são a Postman, na qual seria utilizada para tratar as requisições, realizando os testes das API´s. Para realizar o gerenciamento dos requisitos seria utilizado o JIRA.
2. Abrangência dos Testes:
  * Funcionalidades: As funcionalidades que devem ser testas, seriam as descritas no caso. Que são: o Estoque onde é importante o controle de entrada e saída correto. Anúncios, tendo grande importância seu funcionamento, mantendo a visibilidade dos produtos mais importantes para o cliente, e a promoção da imagem do cliente. Faturamento, onde o controle de receita deve estar sincronizada com as vendas para atualizações em tempo real. Pedidos, os quais devem ser processados para verificação e atualizacão de estoque, tão bem quanto o controle da receita. Por fim o preço, onde deve possuir a garantia de funcionalidade correta, para não causar prejuízos ou inconsistências ao faturamento do cliente.
  * Casos de uso: Para os diversos casos de uso, entre eles o caso de sucesso, seria dado pela atualização imediata do estoque ao realizar uma venda, sincronização de ofertas e preços em tempo real, processamento da solicitação entre o marketplace e e-comerce em tempo hábil, atualização do faturamento em tempo real e suportando grande volume de requisições. Os casos de falha, seriam dados pela falta de atualização do estoque, causando inconsistências. Falta de comunicação entre o marketplace e e-commerce, devido a problemas com as API´s e descrepâncias entre ofertas e valores reais dos produtos. Já se tratando em casos de carga, o problema mais comumente ocasionado seria uma grande massa de requisições, onde viriam a deixar o serviço inoperante.
  * Priorização dos testes: Os testes que devem ser priorizados, seriam em relação a criticidade ao cliente. Partindo da integração do marketplace ao e-commerce, o qual deve ser o primeiro a funcionar, sem isso, não possui vendas. Partindo para testes de faturamento a fim de evitar qualquer dano a receita e portanto o controle de estoque.
3. Execução dos Testes:
  * Ambiente de teste: Os testes seriam realizados em bases de homologação, utilizando dados e registros fictícios para fim de simulação. Testes em bases quentes, também são interessantes para verificar o processamento de requisição das API´s e suporte aos volumes de dados reais.
  * Dados de teste: Seriam utilizados dados ficticios, criando scripts para inserção de dados no banco.
  * Ferramentas de automação: As ferramentas utilizadas seriam para verificar as requisições das API´s, para testar o envio de grande volume de dados a fim de verificar o tanto de carga que é tolerável e ferramenta na qual arquive e organize os logs gerados. 
  * Registro de resultados: Os resultados seriam catalogados conforme os casos de teste, separando pelas ferramentas utilizadas e os resultados obtidos. Assim, apontando os pontos corretos e incorretos, tornando possível uma visualização direta dos pontos que necessitam atenção. Um sistema de gerênciamento tanto quanto uma planilha no excel, seriam úteis para manter este controle. Ao fim, um relatório citando os passos e resultados obtidos para ter uma visão geral do processo e facilitar a tomada de decisão a partir desta documentação.
  
**2° Cenário:**
1. Documentação e Materiais de Apoio:
 * Identificação da documentação: Iria verificar os requistos da integração, acessar a documentação da ferramenta Bling que estiverem disponíveis e se houver, documentação criada pelo time de regra.
 * Mapeamento dos requisitos: Iria mapear os requisitos, fazendo com cada qual, tenha seu caso de teste específico.
 * Utilização de ferramentas: Utilizaria ferramentas como o Postman para validar as requisições e o Jira para realizar o mapeamento e gerenciamento dos requisitos.
2. Abrangência dos Testes:
 * Funcionalidades: Iria realizar a verificação da API com a Bling, analisar o sistema de controle de estoque, verificando as atualizações do mesmo, entra e saída de produtos.
 * Priorização dos testes: A prioridade seria a atualização do estoque em tempo real, a fim de evitar transtornos. A entrada e saída correta dos produtos é essencial para evitar despesa.
3. Execução dos Testes:
 * Dados de teste: Iria realizar a inserção de dados ficticios através do banco de dados.
 * Ferramentas de automação: Seria utilizado uma ferramente para análise das requisições das API´s.
 * Registro de resultados: Os resultados seriam catalogados conforme os casos de teste, separando pelas ferramentas utilizadas e os resultados obtidos. Assim, apontando os pontos corretos e incorretos, tornando possível uma visualização direta dos pontos que necessitam atenção. Um sistema de gerênciamento tanto quanto uma planilha no excel, seriam úteis para manter este controle. Ao fim, um relatório citando os passos e resultados obtidos para ter uma visão geral do processo e facilitar a tomada de decisão a partir desta documentação.
   
**3º Cenário:**
Neste caso, iria verificar a documentação do Mercado Livre a fim de verificar quais as regras impostas nos anúncios apra simular uma situação com um anúncio, a fim de verificar se as requisições estão sendo feitas corretas, se a API está atualizando o estoque para "Pausado (sem estoque)" quando o estoque chega a 0 produtos.

**4º Cenário:**
Para este caso, iria realizar inserção manual via banco de dados e visualizar o cadastro no sistema para ver como se comporta o registro dessa maneira. Posteriormente iria adicionar diretamente pelo sistema para verificar como o registro se comporta. Iria tentar inserir de diversas maneiras dados incorretos, como número no lugar do nome, nome no lugar do email, nome no lugar do cpf e assim por diante, para verificar se o sistema não está atendendo alguma validação necessária. Outro teste, seria verificar se o usuário tem permissão para realizar a edição de informações dos registros.

