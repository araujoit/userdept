# UserDept
Projeto baseado na aula oferecida pelo Nelio, da DevSuperior, desenvolvido com o intuito de aprender/aprofundar os conhecimentos em Spring Boot + Spring Data JPA


## Etapas da Aula

### Criação de Projeto
Definições:
- Spring Boot 2.6.3 (2.6.2 não disponível no momento da criação de projeto)
- Gerenciador de dependências: Maven 
- Empacotamento Jar
- Java 17

Dependências:
- Spring Web
- JPA
- Banco de Dados em memória
- Plugin Maven para evitar conflitos durante os estudos:

```xml
<plugin>
	<groupId>org.apache.maven.plugins</groupId>
	<artifactId>maven-resources-plugin</artifactId>
	<version>3.1.0</version>
</plugin>
```


### Modelo de domínio
Definição de classes conforme desenho do projeto. Entendendo o relacionamento entre elas, a composição de objetos, efetuando a associação de entidades.

### Mapeamento Objeto Relacional - ORM
Resolvido através da utilização das anotações da JPA (Ferramenta de ORM do Java)
*Sempre dar preferência para importar a especificação, não a implementação, pois assim o projeto fica genérico*
No projeto é utilizado o @ManyToOne na propriedade de possui a lista de departamentos, dentro da entidade de usuários, 
sendo que um usuário possui um departamento, mas um departamento possui N usuários

### Banco de dados
- H2: Banco em memória, útil para desenvolvimento
- Configuração e utilização da aplicação WEB de gerenciamento de banco de dados H2
- Para subir dados no banco H2 de forma automatizada: arquivo import.sql, dentro da pasta src/main/resources

### API REST
- Definição dos repositories e controllers, utilizando os métodos fornecidos pelo JPA para manipulação dos arquivos


------------------------
### References
https://github.com/devsuperior/java-web-spring-2022

------------------------
## Conteúdos sugeridos para aprofundar conhecimentos
- https://www.youtube.com/watch?v=jh_T5_o3qKE
- https://www.youtube.com/watch?v=O07XFebgw-g