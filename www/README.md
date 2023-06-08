## Projeto Ulpia - Sistema de Administração de Contratos Jurídicos

O projeto Ulpia é uma aplicação desenvolvida com o framework Spring Boot, que tem como objetivo fornecer uma solução para administração de contratos jurídicos. 

### Configurações do Banco de Dados

O projeto utiliza o Hibernate como ORM (Object-Relational Mapping) e o banco de dados H2 em memória para armazenar os dados dos contratos jurídicos. A seguir estão as configurações relacionadas ao banco no arquivo `application.properties`:

```properties
# JPA
spring.jpa.database-platform=org.hibernate.dialect.H2Dialect
spring.jpa.hibernate.ddl-auto=update

# H2
spring.h2.console.enabled=true
spring.h2.console.path=/h2-console

# DataSource
spring.datasource.driverClassName=org.h2.Driver
spring.datasource.url=jdbc:h2:mem:ulpia
spring.datasource.username=admin
spring.datasource.password=admin
```

### Acesso de Teste

Para facilitar o acesso ao sistema durante o desenvolvimento e testes, você pode utilizar as seguintes informações de usuário:

- Usuário: admin
- Senha: admin

Lembre-se de modificar essas informações ao implantar o projeto em um ambiente de produção.

### Recursos Disponíveis

O projeto Ulpia oferece as seguintes funcionalidades para administrar contratos jurídicos:


### Executando o Projeto

Para executar o projeto Ulpia localmente, siga as instruções abaixo:

1. Certifique-se de ter o Java Development Kit (JDK) instalado na sua máquina.
2. Faça o download do código-fonte do projeto a partir do repositório Git.
3. Importe o projeto em sua IDE de preferência.
4. Aguarde a resolução das dependências do projeto.
5. Execute a classe `UlpiaApplication` para iniciar a aplicação.
6. Acesse o sistema através do navegador usando o endereço `http://localhost:8080`.

Agora você pode começar a administrar seus contratos jurídicos com o Ulpia!

---

Lembre-se de que esta é apenas uma descrição básica do projeto e você pode adicionar mais informações conforme necessário. Certifique-se de fornecer detalhes relevantes sobre as funcionalidades, a arquitetura e quaisquer outras instruções importantes para facilitar o entendimento e a utilização do sistema.