Faça um programa de console em C# que cadastre funcionários em listas, usando apenas while, if, for e Console.Write/ReadLine. Não use classes nem métodos.

Menu: 1-Cadastrar, 2-Listar, 3-Buscar por ID, 4-Editar, 5-Excluir, 0-Sair.

Dados e validações. Cada campo fica em um while até receber um valor válido:

Campo	Regra
Nome	Obrigatório, mínimo de 3 letras, só letras e espaços (conferido com for letra por letra)
Idade	Número inteiro de 18 a 70 (int.TryParse)
E-mail	Precisa ter @, algo antes dele, um . no domínio e nenhum espaço. Não pode repetir (conferido com for na lista).
Salário	Número maior que 0 e até 100.000

O menu também tem que:

recusar letras e números fora de 0 a 5 sem fechar o programa;
bloquear as opções 2 a 5 enquanto a lista estiver vazia;
pedir o ID até achar um que exista, ou 0 para voltar;
na edição, manter o valor atual quando a pessoa aperta ENTER em branco;
na exclusão, aceitar só S ou N como resposta;
na listagem, mostrar a média salarial e quem ganha mais, calculados com for.