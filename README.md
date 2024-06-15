# Gerenciamento-de-Livros
Projeto de final de semestre da Faculdade, afim de por em prática o que aprendemos durante o semestre.
# Como Utilizar o Sistema
O sistema é bastante leve e deve funcionar em computadores e sistemas operacionais antigos, contudo, por ser em Java, é essencial instalá-lo aqui junto do JDK aqui. Além de um aplicativo como o Xampp para fazer o banco de dados local.
# Ferramentas Utilizadas
Este projeto foi feito a base de JAVA utilizando uma biblioteca de Java Swing no qual permite interfaces gráficas de usuário (GUI) em Java. O código foi feito usando o padrão arquitetura CRUD MVC! Esse padrão se baseia em reutilização de código aonde se divide o código em três (3) camadas: Model, Views e Control.

Além disso, o projeto ainda teve a utilização de Banco de Dados MySQL para gerar a tabela Livros aonde serão armazenados os dados dos livros do projeto. Na tabela Livro foram colocados os atributos: ID, Nome, Categoria, Autor, Editora, Sinopse e Data de Publicação, sendo o primeiro um atributo chave conforme imagem abaixo do Modelo Conceitual.

O sistema ainda tem uma documentação em "JAVADOC" em PDF conforme documentado pelos professores do trabalho na pasta de mesmo nome.

 Modelo Conceitual:

![Conceitual](https://github.com/Pedro9Henr/Gerenciamento-de-Livros/assets/144542909/c5351820-9959-46e5-ba75-aa93c03465c5)

 Modelo Lógico:

 ![Lógico](https://github.com/Pedro9Henr/Gerenciamento-de-Livros/assets/144542909/5b3a44bf-c2fe-4a33-9a9f-5185e7c728af)

# Tabela de Livros:

![Livros cortado](https://github.com/Pedro9Henr/Gerenciamento-de-Livros/assets/144542909/1f40abd8-672f-4110-8d03-b845d8071652)

A listagem de livros é feito por meio de uma tabela (JTable). Os dados listados são ID, Nome do Livro, Autor, Editora, Categoria e Ano de Publicação, todos estes vem do banco de dados e são manipulados dentro do Java para ficarem na coluna correta de seus respectivos dados e para formatar a data para o modelo brasileiro (De AAAA/MM/dd para dd/MM/AAAA). Após isso, eles são inseridos na tabela.

# Barra de Pesquisa

![Barra de Pesquisa](https://github.com/Pedro9Henr/Gerenciamento-de-Livros/assets/144542909/37097dd8-6f3c-48f0-b300-be2a4108c595)

Acima da tabela fica uma barra de pesquisa aonde o usuário poderá pesquisar pelo nome do Livro, nome do Autor, Categoria, Editora ou ID do livro. Para isso, basta o usuário pesquisar o que deseja (exemplo na imagem abaixo) e clicar em Buscar que o próprio sistema vai pesquisar no banco de dados essa palavra ou caractere.


![Captura de tela 2024-06-15 140046](https://github.com/Pedro9Henr/Gerenciamento-de-Livros/assets/144542909/f06e249b-bfbc-4356-b705-16dda7db3729)

Acima temos uma imagem mais completa mostrando a tabela e a barra de pesquisa, nesse exemplo podemos ver que o usuário pesquisou na barra de pesquisa a palavra "É ass", no qual o sistema retornou com dois livros, um com "É assim que Acaba" no nome do Livro e outro com "É assim que começa " no nome do Livro. Para cancelar a pesquisa basta clicar no botão Atualizar (não visível na imagem) aonde a tabela será atualizada e voltará para o normal ou deixar a barra de pesquisa em branco e clicar no botão Buscar.

# Menu

![Menu](https://github.com/Pedro9Henr/Gerenciamento-de-Livros/assets/144542909/0087974f-60e2-418b-b3d7-db17a48817fc)

Esta é a primeira tela do sistema, nela terá 4 botões para o usuário escolher: botão Livros que vai para a tela de listar livros para o usuário; botão Login que vai para a tela de Login; botão Sobre aonde o usuário poderá ver os desenvolvedores que desenvolveram o código e por último, o botão Encerrar no qual encerra o sistema.

# Listagem do Usuário

![Livros](https://github.com/Pedro9Henr/Gerenciamento-de-Livros/assets/144542909/3faa8817-9a96-473c-b103-ef3a4e7ecf95)

Nesta tela é aonde estão a tabela e a barra de pesquisa para o usuário. Aqui, além de todas as funcionalidades citadas anteriormente na tabela e na barra de pesquisa, o usuário terá o botão Atualizar aonde ele pode estar atualizando os dados da tabela ou via Timer que atualizará automaticamente a tabela após os 10 primeiros segundos, primeiro 1 minuto e primeiros 10 minutos. Na tela após selecionar um livro clicando nele na tabela, também temos o botão Ver Mais que ao clicá-lo, será aberto uma tela aonde serão mostrados as informações desse livro (Abaixo nessa lista).

# Informações do Livro

![Captura de tela 2024-06-15 141502](https://github.com/Pedro9Henr/Gerenciamento-de-Livros/assets/144542909/79b64835-b172-4fcb-be79-e7445ed4386d)

Nesta tela, serão listados todos os dados do livro selecionado pelo usuário na tela anterior. Entre esses dados têmos o Nome do Livro, Nome do Autor, Categoria, Editora, Sinopse, Data de Publicação. Abaixo na tela têm um botão de Voltar para voltar para a tela anterior.

# Sobre 

![Sobre](https://github.com/Pedro9Henr/Gerenciamento-de-Livros/assets/144542909/31c27e75-74a5-4445-b5c6-b63ee2a39cc8)

Nesta tela são mostrados o Foto dos Desenvolvedores além de seus nomes e RA da faculdade.

# Login

![Login](https://github.com/Pedro9Henr/Gerenciamento-de-Livros/assets/144542909/d0cec97f-ecb3-4c4a-a4f9-9ac0db4582bc)

Nesta tela o usuário poderá fazer login como Administrador para poder adicionar, alterar ou excluir dados dos livros. Para acessar, no campo do usuário deve-se colocar "Admin" (seja com a letra A maiúscula ou minúscula) e no campo "Senha" colocar "123". Caso o usuário tenha colocado de forma correta, aparecerá uma mensagem confirmando o login, caso contrário aparecerá uma mensagem de erro informando login incorreto.

# Listagem do Administrador 

![Livros Admin](https://github.com/Pedro9Henr/Gerenciamento-de-Livros/assets/144542909/66a61fc5-7d52-450f-909d-6f0b47b0b956)

Esta tela tem as mesmas funcionalidades da tabela de listagem citada anteriormente, suas diferenças são a adição de: botão de Criar aonde o administrador vai pra tela de criar livros; botão Alterar, nesse caso o administrador precisa selecionar o livro que deseja alterar seus dados e após isso clicar nesse botão para ir a uma tela aonde poderá alterar os dados dos livros; botão Excluir que segue o mesmo padrão do botão Alterar. O usuário deve selecionar o livro que deseja que seja deletado e por fim clicar no botão que pedirá uma confirmação para realizar a exclusão desse livro. Por último, no botão Ver Mais tem a mesma função do Ver mais do usuário! É aberto uma tela aonde mostra as informações do livro selecionado como mostrado abaixo.

![Informações livros](https://github.com/Pedro9Henr/Gerenciamento-de-Livros/assets/144542909/a75d6293-30b3-4a26-af12-085d4c346148)

# Sair 

![Deslogar](https://github.com/Pedro9Henr/Gerenciamento-de-Livros/assets/144542909/b3ec8330-f7ab-482e-bf12-5a5a93b004c2)

No botão Sair, o sistema emitirá uma mensagem avisando que o usuário sairá da tela de Administrador e precisará fazer login novamente caso saia, então fica a escolha de sair ou ficar na tela para o usuário.

# Excluir Livros

![Excluir livro](https://github.com/Pedro9Henr/Gerenciamento-de-Livros/assets/144542909/184c4974-2960-4174-a848-f98e2e32cbfb)

Após selecionar o livro desejado e clicar no botão Deletar, o sistema mostra essa tela acima! Tela no qual pede confirmação do administrador se ele realmente deseja deletar o livro. Caso o administrador clique em Cancelar, nada será feito. Agora, caso o administrador clique em Excluir, o livro será deletado por completo.

# Alterar Dados do Livro Desejado 

![Captura de tela 2024-06-15 141255](https://github.com/Pedro9Henr/Gerenciamento-de-Livros/assets/144542909/19da858f-8afd-4f61-ade3-d7475547854d)


Após o administrador selecionar o livro desejado e clicar em Alterar, o sistema mostra a tela acima! Nesta tela serão mostrados todos os dados do livro selecionado, como: Nome do Livro, Nome do Autor, Categoria, Editora, Data de Publicação e Sinopse. Para alterar, basta o administrador clicar no campo que deseja alterar e depois clicar em Alterar! Agora, caso o administrador mude de idéia, basta clicar em Voltar que quaisquer alterações serão canceladas. Obs: como alguns campos NÃO podem ficar vazios no banco de dados como o nome do livro, por exemplo; o sistema contornará a caixa de digitação com uma linha vermelha que sumirá apenas quando o administrador clicar em cima! Obs 2: Caso o administrador exceda o número de caracteres permitidos em uma caixa de digitação, exemplo: o nome do livro ultrapassar 60 caracteres, será emitido uma mensagem de erro pedindo para que o administrador reduza a quantidade de caracteres nessa caixa de digitação. Obs 3: A data é formatada para o formato brasileiro (dd/MM/AAAA) ao ser colocada no campo "Data de Publicação".

# Criar Novos Livros 

![Captura de tela 2024-06-15 141415](https://github.com/Pedro9Henr/Gerenciamento-de-Livros/assets/144542909/60342703-3b12-4e9a-b5e3-7568fc79820e)


Nesta tela é aonde serão criados os livros. Aqui o Administrador coloca nome do Livro, nome do Autor, Categoria, Editora, Data de Publicação e Sinopse do livro, lembrando que este último é o único campo que pode ficar vazio. Caso os outros campos estejam vazios será emitido uma mensagem com erro pedindo para que o administrador adicione algum valor para o campo. A data é formatada para o formato brasileiro (dd/MM/AAAA) ao ser colocada no campo "Data de Publicação". Caso o administrador exceda o limite de caracteres em um campo, será retornado uma mensagem de erro pedindo para que apague alguns desses caracteres. Exemplo: se o Nome exceder 60 caracteres, será emitido essa mensagem. Após o administrador preencher todos os dados do livro, basta clicar em Criar que se estiver tudo correto, o livro será criado. Caso mude de ideia, basta clicar em Voltar que nenhum livro será criado.

# Deslogar 

![Deslogar](https://github.com/Pedro9Henr/Gerenciamento-de-Livros/assets/144542909/dd705cff-830a-4975-9d31-b05e6705d5da)

Caso o administrador clique no botão Sair na tela de Listagem como administrador, aparecerá uma caixa de diálogo pedindo uma confirmação do administrador (mostrado acima) se ele têm certeza que quer deslogar e que precisará fazer login de novo para acessar essa tela novamente.










