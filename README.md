# Configuração do Recurso de Idioma no Azure

Para utilizar os recursos de idioma do Azure AI, é necessário criar um recurso de idioma na sua assinatura do Azure. Siga as etapas abaixo para configurar o recurso:

1. Acesse o [portal do Azure](https://portal.azure.com) em outra guia do navegador e faça login com a conta da Microsoft associada à sua assinatura do Azure.

2. Clique no botão **＋Criar um recurso** e pesquise por **Serviço de Idioma**. Selecione **Criar um plano de serviço de idiomas**. Você será direcionado para uma página para selecionar recursos adicionais.

3. Mantenha a seleção padrão e clique em **Continuar** para criar seu recurso.

4. Na página de criação do recurso de idioma, configure-o com as seguintes configurações:
   - **Assinatura**: Selecione sua assinatura do Azure.
   - **Grupo de Recursos**: Escolha ou crie um grupo de recursos com um nome exclusivo.
   - **Região**: Selecione "Leste dos EUA".
   - **Nome**: Insira um nome exclusivo para o recurso.
   - **Nível de Preços**: Escolha entre F0 grátis ou S, se F0 grátis não estiver disponível. Certifique-se de marcar a caixa confirmando que leu e compreendeu todos os termos.

5. Selecione **Revisar + criar** e, em seguida, **Criar**. Aguarde a conclusão da implantação do recurso.

# Configuração do Recurso no Azure AI Language Studio

Para configurar seu recurso no Azure AI Language Studio, siga as etapas abaixo:

1. Acesse o [Language Studio](https://language.cognitive.azure.com) em outra guia do navegador e faça login.

2. Quando solicitado com **Select an Azure resource**, faça as seguintes configurações:
   - **Diretório do Azure**: Deixe como o diretório padrão que você está utilizando.
   - **Assinatura do Azure**: Selecione a assinatura que você está usando.
   - **Tipo de Recurso**: Escolha **Idioma**.
   - **Nome do Recurso**: Selecione o recurso de serviço de idioma que você acabou de criar.

3. Em seguida, selecione **Concluído** para finalizar a configuração.

# Análise de Comentários no Azure Language Studio

Neste tutorial, demonstrarei como utilizar o Azure Language Studio para analisar dois exemplos de comentários fictícios sobre a companhia aérea "SkyGlide".

## Como Utilizar

1. Primeiramente, acesse o [Azure Language Studio](https://language.cognitive.azure.com) em um navegador web.

2. Na página inicial, siga para a seção de "Classificar texto" e clique no bloco "Analisar sentimento e extrair opiniões".

3. Selecione o idioma do texto como "Inglês".

4. Em "Selecione seu recurso do Azure", escolha o recurso previamente criado e configurado em sua assinatura do Azure.

5. Após selecionar o recurso, você pode inserir os comentários fictícios para análise. Utilizaremos os seguintes exemplos:

   - **Exemplo 1**: "A equipe da SkyGlide é extremamente atenciosa e prestativa, garantindo que os passageiros se sintam bem cuidados e confortáveis durante todo o voo. Desde o momento do check-in até o desembarque, os funcionários demonstram profissionalismo e cortesia, proporcionando uma experiência de viagem verdadeiramente agradável."

   ![Resultado primeiro comentario](https://github.com/Lugaus/Desafio-de-Projeto-DIO---Analise-de-Sentimentos-com-Language-Studio-no-Azure-AI/assets/129623426/de641dea-dec7-4d55-bced-eb4824f95fd8)

      No detalhamento de sentimentos, são exibidas palavras-chave relacionadas a sentimentos positivos, destacando uma experiência agradável.

   ![Detalhamento e palavras-chave primeiro comentario](https://github.com/Lugaus/Desafio-de-Projeto-DIO---Analise-de-Sentimentos-com-Language-Studio-no-Azure-AI/assets/129623426/f5a55d38-3fc6-464c-ae1d-d3b7b8e9e2ec)

   - **Exemplo 2**: "Os preços dos voos da SkyGlide tendem a ser mais elevados em comparação com outras companhias aéreas, o que pode ser um obstáculo para alguns passageiros. Embora a qualidade do serviço seja reconhecida, o custo mais alto pode limitar a acessibilidade da companhia aérea para determinados segmentos de clientes em busca de opções mais econômicas."

   ![Resultado segundo comentario](https://github.com/Lugaus/Desafio-de-Projeto-DIO---Analise-de-Sentimentos-com-Language-Studio-no-Azure-AI/assets/129623426/0b1de749-5e94-463b-8205-6b1405e3585f)

      Para o segundo comentário, são relacionadas palavras-chave em sua maioria negativas e neutras.

   ![Detalhamento e palavras-chave segundo comentario](https://github.com/Lugaus/Desafio-de-Projeto-DIO---Analise-de-Sentimentos-com-Language-Studio-no-Azure-AI/assets/129623426/9a8ecf05-266a-4d1a-a4ee-e1973d9dbd1a)

6. Após inserir os comentários, o Azure Language Studio irá analisar o sentimento e extrair opiniões dos mesmos. Observe que os resultados incluem um sentimento geral, seguido por pontuações próximas a três categorias: pontuação positiva, pontuação neutra e pontuação negativa. Cada uma dessas categorias é atribuída uma pontuação entre 0 e 1, indicando a probabilidade do texto fornecido representar um sentimento específico.








