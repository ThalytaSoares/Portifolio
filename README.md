# Bootcamp Qualiters Club

- Criação de testes de API utilizando postman, newmam e newman-htmlextra

# O que é

- Esse repositório foi criado para fixação e aprendizado do conteúdo do Bootcamp de APIRest do manual ao CI/CD

# Tecnologias utilizadas
- Postman version web
- Node version 20.0
- Newman version 6.2
- newman reporter-html

# Documentações
- Doc da API: [Consulte swagger](https://serverest.dev/#/)
  
# Como instalar o ambiente
- Primeiro: Instale o node em seu computador [baixe aqui]:(https://nodejs.org/en/download)
- Segundo: Realize a instalação do newman de forma global [baixe aqui a dependencia:] (https://www.npmjs.com/package/newman)
  ```
  npm install -g newman
  ```
- Terceiro: Realize a instalação das dependencias dos relatórios (opcional) [newman-reporter-html (https://www.npmjs.com/package/newman-reporter-html)
  ```
  npm install -g newman-reporter-html
  ```
 
# Como rodar os testes

### Pelo postman web ou desktop
- Import a collection e o environment
- Execute os teste de forma manual ou automatizada
  
### Pelo Newman
- Abra o console de preferência
- Execute a seguinte linha de comando para rodar os testes
  ```
  newman run ServeRest.postman_collection.json -e ServeRest-env.postman_environment.json -r cli
  ```
- Execute os testes com relatório
  ```
  newman run ServeRest.postman_collection.json -e ServeRest-env.postman_environment.json -r cli,htmlextra
  ```
### Report
- Se você optou por rodar os testes com o report html-extra, você gerou um arquivo html com o resultado dos testes e para verificar as validações, você pode abrir a pasta **newman** que foi criada no local em que os arquivos de collection e environment se encontram.
