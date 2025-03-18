# ai-search-microsoft-azure
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

##Passo 9
✅Agora voltamos ao AI Search, através do campo de busca.

![image](https://github.com/user-attachments/assets/bc4b500f-604d-4f0d-b252-050926797800)


✅ Selecione o serviço criado anteriormente e clique em **"Importar dados"**

![image](https://github.com/user-attachments/assets/cfc38ad6-2adf-46d4-91b1-6645b361f6c7)


## Passo 10
✅ Selecione **"Armazenamento de Blob do Azure"**

Preencha os dados conforme os passos na imagem e clique em **"próximo"**.

A informações não presentes nos passos já vêm preenchidas, ou devem ser deixadas em branco.

![image](https://github.com/user-attachments/assets/a4d0c07e-56ca-4fa6-83a2-89c8be92b71a)

✅ Na aba "Add Cognitive skills (optional)", em "Attach AI Services", selecione seu recurso.

![image](https://github.com/user-attachments/assets/949cf964-deae-4ecf-b023-34f13a830ee2)


















