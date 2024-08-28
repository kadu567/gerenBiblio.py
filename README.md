# Documentação do Programa de Gerenciamento de Biblioteca
1. Documentação das Classes e Métodos

1.1 Classe ItemBiblioteca
Descrição: Classe base que representa um item básico na biblioteca.
Atributos:
titulo: Título do item (pode ser o nome do livro ou do usuário).

1.2 Classe Livro
Descrição: Representa um livro na biblioteca. Herda de ItemBiblioteca.
Atributos:
titulo: Título do livro.
autor: Autor do livro.
isbn: Código ISBN do livro.
Métodos: Herda os métodos da classe base.

1.3 Classe Usuario
Descrição: Representa um usuário da biblioteca. Herda de ItemBiblioteca.
Atributos:
nome: Nome do usuário.
matricula: Número de matrícula do usuário.
Métodos: Herda os métodos da classe base.

1.4 Classe Biblioteca
Descrição: Gerencia os livros e usuários cadastrados na biblioteca.
Atributos:
livros: Lista de livros cadastrados.
usuarios: Lista de usuários cadastrados.
Métodos:
adicionar_livro(livro): Adiciona um livro à lista de livros.
adicionar_usuario(usuario): Adiciona um usuário à lista de usuários.

1.5 Classe GerenciadorDePedidos
Descrição: Gerencia os pedidos de empréstimo de livros.
Atributos:
biblioteca: Referência à biblioteca que contém os livros e usuários.
pedidos: Lista de pedidos de livros.
Métodos:
solicitar_livro(usuario, livro): Registra um pedido de empréstimo se o livro estiver disponível na biblioteca.

1.6 Classe BibliotecaApp
Descrição: Interface gráfica do programa usando tkinter.
Atributos:
root: Janela principal do tkinter.
biblioteca: Instância da classe Biblioteca para gerenciar livros e usuários.
main_frame: Frame principal que contém os botões de navegação.
Métodos:
cadastro_livro(): Abre a tela para cadastrar um novo livro.
cadastro_usuario(): Abre a tela para cadastrar um novo usuário.
visualizar_livros(): Exibe a lista de livros cadastrados.
visualizar_usuarios(): Exibe a lista de usuários cadastrados.
voltar(frame): Volta para a tela principal de navegação.

2. Descrição das Funcionalidades

2.1 Cadastro de Livros
Permite ao usuário cadastrar novos livros na biblioteca inserindo o título, autor e ISBN.

2.2 Cadastro de Usuários
Permite ao usuário cadastrar novos usuários na biblioteca inserindo o nome e a matrícula.

2.3 Visualização de Livros
Exibe a lista de todos os livros cadastrados na biblioteca, mostrando título, autor e ISBN.

2.4 Visualização de Usuários
Exibe a lista de todos os usuários cadastrados, mostrando nome e matrícula.

2.5 Navegação Entre Telas
O programa permite ao usuário navegar entre diferentes telas, como cadastro de livros, cadastro de usuários e visualização de registros.

3. Roadmap de Execução

3.1 Inicialização do Programa
O programa começa criando uma instância da classe BibliotecaApp, que configura a interface gráfica e exibe a tela principal.

3.2 Cadastro de Livro ou Usuário
Quando o usuário clica em "Cadastrar Livro" ou "Cadastrar Usuário", a tela correspondente é exibida. Após preencher os dados, o usuário clica em "Salvar", e os dados são armazenados na biblioteca.

3.3 Visualização de Livros ou Usuários
Ao clicar em "Visualizar Livros" ou "Visualizar Usuários", uma lista dos livros ou usuários cadastrados é exibida.

3.4 Retorno à Tela Principal
A qualquer momento, o usuário pode voltar à tela principal clicando no botão "Voltar".

4. Manual de Instalação e Uso

4.1 Dependências
tkinter: Biblioteca padrão para criação de interfaces gráficas no Python. Não precisa ser instalada separadamente.

4.2 Instalação
Certifique-se de ter o Python instalado. O tkinter já está incluído na maioria das distribuições Python. Caso precise instalar o Python, você pode baixá-lo no site oficial.

4.3 Inicialização
Para iniciar o programa, abra o terminal e execute o seguinte comando:
Copiar código
python nome_do_arquivo.py

4.4 Uso
Na tela principal, escolha entre cadastrar livros, cadastrar usuários, visualizar livros ou visualizar usuários.
Siga as instruções na tela para realizar cada ação.
Use o botão "Voltar" para retornar à tela principal sempre que necessário.
