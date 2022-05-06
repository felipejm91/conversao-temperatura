# conversao-temperatura
Repositório para Curso Kubedev

=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*

PROCEDIMENTOS PARA CRIAÇÃO DA IMAGEM E EXECUÇÃO DO CONTAINER

1º) Criar o documento "dockerfile" para documentar a criação da imagem da aplicação

2º)Executar comando para a criação da imagem, criando as versões seguindo as boas práticas

      docker build -t felipejm91/conversao-temperatura .
  
      docker build -t felipejm91/conversao-temperatura:v1 .
 
3º)Executar comando para criação do container utilizando a imagem criada
  
      docker run -d --name conversao -p 8080:8080 felipejm91/conversao-temperatura:v1
  
4º)Acessar a aplicação
  
      Abrir um navegador e digitar o caminho "localhost:8080"
  
5º)Aplicação rodando em container
