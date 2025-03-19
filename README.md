# AI-search-microsoft-azure
✅ Passo a passo da atividade Azure Cognitive Search: Utilizando AI Search para indexação e consulta de Dados da plataforma Dio.
Documentação: https://aka.ms/ai900-ai-search

## Passo 1  
✅ Abrir a página do [Portal Azure](https://portal.azure.com/#home), buscar e selecionar o **"AI Search"**.

![image](https://github.com/user-attachments/assets/60b60dd7-5480-4e17-9fb2-2bfe6262db60)

## Passo 2  
✅ Clique em **"Create"** para criar um novo search service e preencha as informações de acordo com a ordem da imagem abaixo, escolhendo **"Básico"** em camada de preços. Após isso, pode clicar em **"Revisar + Criar"**:

![image](https://github.com/user-attachments/assets/4af8f760-e76f-483f-acfb-108110b99776)

✅ Depois que as informações são validadas, é aberta uma tela com as configurações. Clique em "Create".

![image](https://github.com/user-attachments/assets/ce2ff531-0d30-4bad-bda3-e1e6cbddac2a)

✅ Depois da confirmação de criação, clique em "Ir para o recurso":

![image](https://github.com/user-attachments/assets/aaeb0d08-5965-4763-b2a3-a98207830ebf)


## Passo 3
✅ Precisamos criar agora um recurso de IA.

De volta à Home do Portal Azure, no menu lateral, clique em **"Create a resource"**, escolha **"AI + Machine Learning"**, depois **"Azure AI Services"**

![image](https://github.com/user-attachments/assets/0e23bcba-eae3-4fae-b01c-3b3c7b26c308)

## Passo 4
✅ Preencha com as informações segundo a imagem abaixo. Clique em **"Examinar + Criar"**

![image](https://github.com/user-attachments/assets/281cd8db-8af0-426b-9a38-92f22b33e59f)

✅ Agora clique em **"Criar"**

![image](https://github.com/user-attachments/assets/32f3635c-8d75-4df4-b126-dfbb073cbf62)

✅ Aguarde até a finalização da criação do recurso.

![image](https://github.com/user-attachments/assets/115c5c2e-5a0e-4e50-86bf-00d11d5332f8)


## Passo 5
✅ Agora criaremos uma conta de armazenamento.

Volte à home do Portal Azure, busque e selecione **"storage accounts ou contas de armazenamento"** e clique em **"Criar"**

![image](https://github.com/user-attachments/assets/8e6dc8d2-8704-482c-995f-adba3257ab7d)

✅ Preencha os dados do formulário abaixo. 

Em **"Redundância"** escolha **"LRS (armazenamento com redundância local)"**

Após isso clique em **"Examinar + criar"**

![image](https://github.com/user-attachments/assets/89afe2b1-a157-4c3d-9347-10140ba90929)

![image](https://github.com/user-attachments/assets/33eb1af0-e032-4546-880b-5297808dbbce)

✅ Depois de criada clique em **"Ir para o recurso"** 

![image](https://github.com/user-attachments/assets/9b72ea06-f137-415a-94c4-f37bbefcace5)

## Passo 6
✅ Na tela da **"Conta de armazenamento"**, no menu lateral esquerdo, procure e selecione a opção **"Configuração"**. 
Clique para habilitar a opção **"Permitir acesso anônimo ao Blob"** conforme imagem e clique em **"salvar"**.

![image](https://github.com/user-attachments/assets/a0fa676a-2b13-4cf6-be12-7bf8b36cf93f)

## Passo 7
✅ No menu lateral esquerdo, clique em **"Armazenamento de dados > Contêineres"**, e então  em **"+ contêiner"**, que abrirá uma aba lateral. Selecione o campo **"Nível de acesso anônimo"** com a opção **"Contêiner(acesso de leitura anônima para contêineres e blobs)"**. Depois clique em **"Criar"**.

![image](https://github.com/user-attachments/assets/5af1bb49-be57-476b-96a8-a90f9788af92)

## Passo 8
✅Em um novo navegador, faça o download do zip contido no link fornecido na documentação: https://aka.ms/mslearn-coffee-reviews, e extraia os arquivos em uma pasta **"reviews"**
Clique então em upload, que abrirá uma aba lateral. Selecione então todos os arquivos descompactados, e clique em **"upload"**


![image](https://github.com/user-attachments/assets/ead39c8c-ff60-4ded-a067-b1d65a2c8096)


✅ Arquivos carregados no contêiner **"coffeereviews"**

![image](https://github.com/user-attachments/assets/a65dbab8-d6fa-44e0-8cb3-3f0b152b94c9)

## Passo 9
✅Agora voltamos ao AI Search, através do campo de busca.

![image](https://github.com/user-attachments/assets/bc4b500f-604d-4f0d-b252-050926797800)


✅ Selecione o serviço criado anteriormente e clique em **"Importar dados"**

![image](https://github.com/user-attachments/assets/cfc38ad6-2adf-46d4-91b1-6645b361f6c7)


## Passo 10
✅ Selecione **"Armazenamento de Blob do Azure"**

Preencha os dados conforme os passos na imagem e clique em **"próximo"**.

A informações não presentes nos passos já vêm preenchidas, ou devem ser deixadas em branco.

![image](https://github.com/user-attachments/assets/a4d0c07e-56ca-4fa6-83a2-89c8be92b71a)

✅ Na aba **"Add Cognitive skills (optional)"**, em **"Attach AI Services"**, selecione seu recurso.

![image](https://github.com/user-attachments/assets/949cf964-deae-4ecf-b023-34f13a830ee2)

✅ Em **"Adicionar enriquecimentos"** preencher conforme imagem abaixo

![image](https://github.com/user-attachments/assets/b3ad2759-c11f-431b-9472-c0b5552c1f59)

![image](https://github.com/user-attachments/assets/a26b51e2-87c4-4dfe-acf6-46f7f80b9bf6)

✅ Em **"Salvar os enriquecimentos em um repositório de conhecimento"**, selecione **"Projeções de imagem"**.
✅ Em **"Escolher uma conexão existente"** selecione o storage criado anteriormente.

![image](https://github.com/user-attachments/assets/dd78c280-97a5-49cd-8a78-c62de599f562)

✅ Clique em **"Próximo: Personalizar índice de destino"**

## Passo 11

✅ Na aba **"Personalizar índice de destino"**, preencha conforme imagem abaixo, em seguida clique em **"Próximo criar um indexador"**:

![image](https://github.com/user-attachments/assets/b1132710-54f6-4c35-8ade-0af13093a4f6)


## Passo 12
✅ Em **"Criar um indexador"**, preencha conforme imagem abaixo:

![image](https://github.com/user-attachments/assets/2550405d-1e91-4d73-a96b-57875bbdea02)

✅ Abra a aba **"Opções avançadas"**, marque a opção **"Chaves de Codificação de Base 64"**, e clique em **"Enviar"**

![image](https://github.com/user-attachments/assets/b7dae113-072b-4c26-9081-68ccf13c58f0)

## Passo 13
✅ Abrir o Azure AI Services| Ai Search, e clicar em **"Explorador de pesquisa"**

![image](https://github.com/user-attachments/assets/7bb4de51-0588-4cb4-9354-ed19cb18b141)

## Passo 14
✅ Em **"Explorador de pesquisa"**, inclua a query fornecida pela documentação **"search=*&$count=true"**, e clique em **"pesquisar"**

![image](https://github.com/user-attachments/assets/c9f9b722-7c65-40b0-93e6-688352d490b8)

✅ Agora filtramos pela localização **"search=locations:'Chicago'"** e ele vai trazer as reviews com os sentimentos de cada.

```json
{
  "@odata.context": "https://lab-ia-search-gui.search.windows.net/indexes('azureblob-index')/$metadata#docs(*)",
  "@odata.count": 3,
  "value": [
    {
      "@search.score": 3.5609007,
      "content": "Review: I often make Fourth Coffee my meeting spot for my client meetings weekday mornings. I own a small business and the folks who work at Fourth Coffee are always very friendly. It leaves a good impression on my clients. There are also plenty of drink selections, good wi-fi, and seating. Some of my favorite coffees are the lavender honey latte and, in the winter, the apple-chai latte. There are delicious baked goods offered as well. \nDate: October 21, 2018\nLocation: Chicago, Illinois",
      "metadata_storage_path": "aHR0cHM6Ly9zdG9yYWdlZ3VpdWJhLmJsb2IuY29yZS53aW5kb3dzLm5ldC9jb2ZmZWVyZXZpZXdzL3Jldmlldy01LmRvY3g1",
      "locations": ["Fourth Coffee", "Chicago", "Illinois"],
      "keyphrases": ["delicious baked goods", "lavender honey latte", "apple-chai latte", "Fourth Coffee"],
      "sentiment": "[\"positive\"]",
      "imageTags": ["clothing", "person", "furniture", "human face"],
      "imageCaption": [{ "text": "a woman showing a woman something on a tablet", "confidence": 0.513512134552002 }]
    },
    {
      "@search.score": 1.0562487,
      "content": "Review: The coffee tastings every Wednesday afternoon are so fun. Each month there is a new drink theme. You do need to book a spot in advance to attend. It is very worth it! I also love their local music. Fourth Coffee brings in rising artists every weekend. I like to head over there mid-afternoon on weekdays when it’s not too busy and get a slice of pie or their seasonal baked goods. \nDate: August 13, 2018\nLocation: Chicago, Illinois",
      "metadata_storage_path": "aHR0cHM6Ly9zdG9yYWdlZ3VpdWJhLmJsb2IuY29yZS53aW5kb3dzLm5ldC9jb2ZmZWVyZXZpZXdzL3Jldmlldy00LmRvY3g1",
      "locations": ["Chicago", "Illinois"],
      "keyphrases": ["new drink theme", "seasonal baked goods", "coffee tastings", "local music", "Fourth Coffee"],
      "sentiment": "[\"positive\"]",
      "imageTags": ["food", "chocolate", "table", "cup", "coffee"],
      "imageCaption": [{ "text": "a group of small cups with brown liquid in them", "confidence": 0.39556050300598145 }]
    },
    {
      "@search.score": 0.96866095,
      "content": "Review: Today I was truly disappointed with how long I had to wait for the pastries I ordered ahead of time. When I got my box, some of the pastries seemed stale. Terrible experience! \nDate: October 23, 2018\nLocation: Chicago, Illinois",
      "metadata_storage_path": "aHR0cHM6Ly9zdG9yYWdlZ3VpdWJhLmJsb2IuY29yZS53aW5kb3dzLm5ldC9jb2ZmZWVyZXZpZXdzL3Jldmlldy04LmRvY3g1",
      "locations": ["Chicago", "Illinois"],
      "keyphrases": ["Terrible experience", "Review", "pastries", "time", "box"],
      "sentiment": "[\"negative\"]",
      "imageTags": [],
      "imageCaption": []
    }
  ]
}
```

✅ Agora filtramos pelo sentimento negativo **"search=sentiment:'negative'"**


```json
{
  "@odata.context": "https://lab-ia-search-gui.search.windows.net/indexes('azureblob-index')/$metadata#docs(*)",
  "@odata.count": 1,
  "value": [
    {
      "@search.score": 0.2876821,
      "content": "Review: Today I was truly disappointed with how long I had to wait for the pastries I ordered ahead of time. When I got my box, some of the pastries seemed stale. Terrible experience!  \nDate: October 23, 2018\nLocation: Chicago, Illinois \n\n",
      "metadata_storage_path": "aHR0cHM6Ly9zdG9yYWdlZ3VpdWJhLmJsb2IuY29yZS53aW5kb3dzLm5ldC9jb2ZmZWVyZXZpZXdzL3Jldmlldy04LmRvY3g1",
      "locations": [
        "Chicago",
        "Illinois"
      ],
      "keyphrases": [
        "Terrible experience",
        "Review",
        "pastries",
        "time",
        "box",
        "Date",
        "October",
        "Location",
        "Chicago",
        "Illinois"
      ],
      "sentiment": "[\"negative\"]",
      "merged_content": "Review: Today I was truly disappointed with how long I had to wait for the pastries I ordered ahead of time. When I got my box, some of the pastries seemed stale. Terrible experience!  \nDate: October 23, 2018\nLocation: Chicago, Illinois \n\n",
      "text": [],
      "layoutText": [],
      "imageTags": [],
      "imageCaption": []
    }
  ]
}
```
## Comentários

✅ A ferramenta se mostra muito útil para negócios que oferecem serviços. Sua análise é bastante eficiente na identificação de frases-chave, sentimentos e localização, além de integrar essas informações de forma precisa na busca. Um exemplo prático é a possibilidade de entender melhor os motivos de avaliações negativas, já que as frases-chave destacam esses pontos. Isso facilita a identificação e solução de problemas que podem estar gerando insatisfação nos clientes.























