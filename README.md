# Receitas
Sistema para auxiliar a encontrar receitas baseadas nos ingredientes que a pessoa já tem em casa.

#### Time:
* Breno de Castro Pimenta
* Luiz Felipe Nery 
* Pedro Fonseca Wildemberg
* Rafael Gonçalves de Oliveira

#### Tecnologias:
* **Back-end**: Django
* **Front-end**: Vue.js
* **DataBase**: PostgreSQL

---




## Papéis

* Breno:  Back-end
* Luiz:  Back-end
* Pedro: Front-end
* Rafael: Front-end


## Backlog

### Backlog do Produto

* Como usuário, quero buscar receitas por nome.
* Como usuário, quero buscar receitas que usem o que tenho na geladeira.
* Como usuário, quero escolher a forma de visualização dos resultados.
* Como usuário, quero ter mais informações sobre uma receita.
* Como usuário, quero uma página inicial com receitas relevantes.
* Como usuário quero fazer buscas avançadas (com filtros, por tipos de receita, por avaliação, por porções, por tempo de preparo).
* Como desenvolvedor, quero obter feedbacks dos usuários a respeito dos resultados das buscas.
* Como usuário, quero criar uma conta.
* Como usuário, quero fazer login.
* Como usuário, quero salvar minhas receitas favoritas.
* Como usuário, quero resultados personalizados. (Extra)
* Como usuário, quero a opção de visualizar a aplicação em Dark Mode.


### Backlog Sprint 1

Histórias: 0, 1, 2, 3 e 4.


1. (Fazer setup do ambiente, banco de dados, etc)
    1. Adicionar linter Front (Rafael)
    2. Adicionar linter Back (Luiz)
    3. Adicionar elasticsearch no projeto (Luiz)
        1. caso seja muito difícil usar essa ferramenta, usar um banco de dados padrão
        2. https://sunscrapers.com/blog/how-to-use-elasticsearch-with-django/
    4. Conteinerizar todo o ambiente (Breno)
    5. Inicializar o projeto django (Breno)
    6. Integrar elasticsearch com o django (Breno / Luiz)
    7. Criar regras no repositório para seguir o SCM definido. (Breno / Rafael)
2. Como usuário, quero buscar receitas por nome.
    1. Adicionar receitas no elasticsearch (Luiz)
    2. Criar página inicial com um componente contendo duas abas. (Rafael)
    3. Criar componente na primeira aba para realizar busca por nome de receita. (Rafael)
    4. Esse componente deve possuir um campo para o usuário entrar com o texto a ser pesquisado.
    5. Criar um componente para listar as receitas que serão retornadas pela API. (Pedro)
    6. Criar endpoint com requisição GET (Breno)
    7. Essa requisição deve aceitar um parâmetro do tipo string, que será utilizado como filtro para receitas, e retornar uma lista de receitas.
    8. Criar busca no elasticsearch para receitas (Luiz)
3. Como usuário, quero buscar receitas que usem o que tenho na geladeira. 
    1. Criar componente da segunda aba de pesquisa para informar os ingredientes a serem adicionados na busca. (Pedro)
4. Como usuário, quero escolher a forma de visualização dos resultados. 
    1. Fornecer 2 formas de visualização: grid com imagens e lista. (Pedro)
        1. Grid como default (?), botão para alternar entre formas.
5. Como usuário, quero ter mais informações sobre uma receita.
    1. Ao clicar na receita, o usuário deve ser redirecionado para a página original da receita. (Rafael)


