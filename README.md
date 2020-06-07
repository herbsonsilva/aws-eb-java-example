# aws-eb-java-example
Exemplo simples de código 'Hello World' em Java para deploy na AWS com Elastic Beanstalk.

<h1 align="center">
    MBA em Full Stack Web Development<br />
    Módulo: Cloud Computing
</h1>

<h4 align="center">
  
</h4>

<p align="center">
  <img alt="GitHub top language" src="https://img.shields.io/github/languages/top/herbsonsilva/eb-java-example.svg">
  
  <img alt="GitHub language count" src="https://img.shields.io/github/languages/count/herbsonsilva/eb-java-example.svg">
  
  <a href="https://www.codacy.com/app/herbsonsilva/eb-java-example?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=herbsonsilva/eb-java-example&amp;utm_campaign=Badge_Grade">
    <img alt="Codacy grade" src="https://img.shields.io/codacy/grade/4f87fc059ec846118f2ef2950200b13a.svg">
  </a>
  
  <img alt="Repository size" src="https://img.shields.io/github/repo-size/herbsonsilva/eb-java-example.svg">
  <a href="https://github.com/herbsonsilva/eb-java-example/commits/master">
    <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/herbsonsilva/eb-java-example.svg">
  </a>
  
  <a href="https://github.com/herbsonsilva/eb-java-example/issues">
    <img alt="Repository issues" src="https://img.shields.io/github/issues/herbsonsilva/eb-java-example.svg">
  </a>
  
  <img alt="GitHub" src="https://img.shields.io/github/license/herbsonsilva/eb-java-example.svg"> 
  
</p>

<p align="center">
  <a href="#rocket-tecnologias">Tecnologias</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#memo-notas">Notas</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#warning-pré-requisitos">Pré-requisitos</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#information_source-como-usar">Como usar</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#page_facing_up-licença">Licença</a>
</p>

## :rocket: Tecnologias

Este projeto foi desenvolvido no módulo de Cloud Computing do curso de [MBA em Full Stack Web Development][curso] usando as seguintes tecnologias:

This project was developed in the Cloud Computing module of the Full Stack Web Development MBA course using the following technologies:

-  [Spring Boot](https://spring.io/projects/spring-boot)
-  [Spring Tools 4](https://spring.io/tools)

## :memo: Notas

O Elastic Beanstalk executa o aplicativo na porta 5000, enquanto o Spring Boot é executado na porta 8080. Pensando nisso, configuramos nossa aplicação para rodar na porta 5000 adicionando o código ```server.port=5000``` no arquivo ```application.properties``` da pasta ```/src/main/resources/```

Elastic Beanstalk runs the application on port 5000, while Spring Boot runs on port 8080. With that in mind, we configured our application to run on port 5000 by adding the code ```server.port=5000``` in the ```application.properties``` file in the folder ```/src/main/resources/```

## :warning: Pré-requisitos

Antes de fazer upload do seu código, será necessário exportá-lo como um arquivo JAR. Vá para a pasta raiz do aplicativo e digite o seguinte comando:

Before you upload your code you will need to export it as a JAR file. Go inside your application folder and type the following command:

```bash
# Exporte o arquivo JAR | Export the JAR file
$ ./mvnw package -DskipTests
```

## :information_source: Como usar

Para clonar e executar esta aplicação, você precisará do [Git](https://git-scm.com) instalado no seu computador. Na sua linha de comando digite:

To clone and run this application, you will need Git installed on your computer. At your command line type:

```bash
# Para rodar a aplicação | To run the application
$ ./mvnw spring-boot:run
```

Se você acessar [```http://localhost:5000/```](http://localhost:5000/) no seu navegador web, verá a seguinte mensagem:

If you go to ```http://localhost:5000/``` in your web browser, you will see the following message:

```
Hello World!
```

**Implantando o aplicativo no AWS Elastic Beanstalk** <br/>
Deploying the application to AWS Elastic Beanstalk

Após fazer login no console da AWS, vá para 'Serviços' e digite 'Elastic Beanstalk' na pesquisa. Clique nele e você será redirecionado para uma página de boas-vindas. Clique no botão 'Iniciar' para começar a criar seu aplicativo na nuvem.

Você criará um aplicativo da web. Coloque as seguintes informações para os campos abaixo:

**Nome do aplicativo:** hello-world <br/>
**Plataforma:** Java <br/>
**Código do aplicativo:** faça o upload do seu código <br/>

Faça o upload do arquivo ```hello-world-0.0.1-SNAPSHOT.jar``` que está pasta de ```target``` do projeto.

Quando o upload terminar, clique no botão 'Criar aplicativo'. A AWS começará a criar o ambiente, exibindo os logs do que está acontecendo no processo.

Depois que o ambiente estiver configurado, a AWS o redirecionará para o 'Painel'. Acima do menu do painel, você encontrará a URL para acessar o aplicativo. Abra-o em uma nova guia e ele carregará a página na web.

Isso é tudo pessoal!

--

After logging into the AWS console, go to Services and type Elastic Beanstalk in the search. Click on it, and it will redirect you to a Welcome page. Click on the Get started button to start creating your application in the cloud.

You will create a web application. Enter the following information for the fields below:

Application name: hello-world
Platform: Java
Application code: upload your code

Upload the file ```hello-world-0.0.1-SNAPSHOT.jar``` under the ```target``` folder.

When the upload completes, click on the Create application button. AWS will start to create the environment, displaying the logs of what is happening in the process.

Once the environment is set up, AWS will redirect you to the Dashboard. Above the dashboard menu, you’ll find the URL to access the application. Open it in a new tab, and it will load your web page.

That's all folk! 

## :page_facing_up: Licença

Este projeto está sob a licença MIT. Consulte [LICENÇA](https://github.com/herbsonsilva/aws-eb-java-example/blob/master/LICENSE) para obter mais informações.

This project is under the MIT license. See the [LICENSE](LICENSE) for more information.

---

Made with ♥ by Herbson Silva :wave: [Get in touch!][linkedin]

[curso]: https://www.iesp.edu.br/cursos/pos-graduacao/mba-em-full-stack-web-development
[linkedin]: https://www.linkedin.com/in/herbsonsilva/
