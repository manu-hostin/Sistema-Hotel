Sistema de Gestão de Hotel
Descrição do Projeto

Este sistema foi desenvolvido para gerir as operações de um hotel. Ele permite o cadastro de hóspedes, quartos e reservas, além de oferecer funcionalidades para listar, pesquisar, editar e cancelar dados no sistema. O sistema foi construído em Java, utilizando conceitos de orientação a objetos, como classes, herança, polimorfismo, agregação e encapsulamento.

Funcionalidades do Sistema:

Cadastro de Hóspedes: Cadastro de informações do hóspede, como nome, documento e telefone.

Cadastro de Quartos: Cadastro de quartos disponíveis no hotel, incluindo número, tipo e preço.

Cadastro de Reservas: Realização de reservas, associando hóspedes a quartos com datas de entrada e saída.

Listagem: Listagem de todos os hóspedes, quartos e reservas registradas no sistema.

Pesquisa: Pesquisa de hóspedes por nome, quartos por tipo e reservas por nome do hóspede.

Edição de Hóspede: Atualização dos dados de um hóspede já cadastrado.

Cancelamento de Reserva: Cancelamento de uma reserva existente.

Saída do Sistema: Opção para sair do sistema de gestão.

Desafios Implementados:

Classe Abstrata Pessoa: Criação de uma classe abstrata Pessoa que contém atributos e métodos comuns a todas as pessoas do sistema, como os hóspedes.

Agregação com Serviços: A classe Reserva agrega um ou mais serviços, como café da manhã ou lavanderia, permitindo a customização das reservas com serviços adicionais.

Estrutura do Projeto

O código foi organizado em pacotes para facilitar a manutenção e escalabilidade:

model: Contém as classes que representam as entidades do sistema (Hóspede, Quarto, Reserva, Serviço).

view: Responsável pela interface do usuário e exibição das opções no console.

service: Contém as lógicas de negócios do sistema, como manipulação de listas e operações de cadastro, pesquisa, edição e cancelamento.

Requisitos Técnicos

Java 8+.

IDE: Qualquer IDE que suporte Java, como Eclipse, IntelliJ ou VS Code.

Bibliotecas: Nenhuma biblioteca externa foi utilizada. Apenas a biblioteca padrão do Java.

Como Rodar o Sistema
1. Clone o repositório:
```git clone https://github.com/seu-usuario/sistema-hotel.git```

2. Compile o código:

Na raiz do projeto, execute o comando para compilar:

javac -d bin src/**/*.java

3. Execute o sistema:

Na pasta bin, execute o sistema com o comando:

java view.Menu

Isso abrirá o menu principal do sistema

Conceitos Utilizados

Encapsulamento: Todos os atributos das classes são privados e acessados por meio de métodos getters e setters.

Herança: Hóspede herda de uma classe abstrata Pessoa, que contém dados comuns.

Agregação: A classe Reserva contém uma lista de objetos Servico como parte de sua estrutura.

Polimorfismo e instanceof: O sistema pode verificar o tipo de objeto em tempo de execução utilizando instanceof quando necessário.

Tratamento de Erros

Foi implementado tratamento de exceções com try/catch para capturar entradas inválidas do usuário, como valores numéricos fora do esperado ou formato de datas incorreto.

Melhorias Futuras

Persistência de Dados: Integrar com um banco de dados para persistir as informações.

Interface Gráfica: Substituir a interface de console por uma interface gráfica (GUI).

Autenticação de Usuário: Implementar um sistema de login para acesso restrito.
