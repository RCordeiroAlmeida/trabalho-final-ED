# trabalho-final-ED
Este é o meu trabalho final do CCR de Estrutura de dados


O Sistema de Agenda
Você foi contratado pela UFFS para criar um sistema com o qual os professores possam controlar alguns detalhes de suas agendas para melhor atender aos estudantes. A universidade já definiu o que é mais importante, para que você comece a criar a estrutura do sistema. Esta estrutura deve obrigatoriamente armazenar os eventos em uma estrutura de lista encadeada simples.

O programa se chamará UFFSAgenda.
Organização do código:
Crie uma estrutura Evento que contém Data, Hora, Duração e descrição do evento (veja a sugestão de struct ao final deste documento):
Exemplo:
Código: 1
Data: 24/12/2022
Hora: 19:00
Duração: 3.5
Descrição: Jantar de Natal no Palácio do Alvorada


Crie a agenda deverá permitir a inclusão, exclusão, consulta e alteração de compromissos cadastrados. A consulta deverá ser por data (aparecem todos os eventos na data informada) ou por data e hora, aparecem todos os eventos cadastrados na data e hora informados. Deverá existir um menu para o usuário escolher a ação sobre a agenda. Por exemplo:
Incluir
Consultar
Alterar
Excluir
Listar todos
Sair

O que acontece com cada item do menu:
Incluir: permite que um compromisso seja incluído na agenda. Verificar se já existe um compromisso agendado para a mesma data e horário. 
Consultar: permite fazer consultas de duas formas: pela data e pela data e hora. No caso de apenas pela data, listar todos os compromissos naquela data. Para data e hora, apenas o compromisso agendado para a data e hora informados. Apresentar a mensagem “Agenda Vazia” caso não existam compromissos para a consulta realizada.
Alterar: permite alterar a descrição e a duração de um compromisso. O usuário digita a data e hora do compromisso a ser alterado. Apresentar a mensagem “Compromisso não encontrado” caso não exista compromisso para a data e hora informados.
Excluir: permite excluir um compromisso. A implementação é similar ao da opção Alterar, exceto que o compromisso é excluído da lista.
Listar todos: lista todos os compromissos da agenda.
Sair: finaliza o programa.


Dicas

Você pode utilizar as seguintes estruturas para implementar seu sistema
struct _data {
   int dia;
   int mes;
   int ano;
   int hora;
   int minuto;


};
typedef struct _data Data;


struct _evento {
   int codigo;
   Data dataEvento;
   float duracao;
   char descricao[100];
   struct _evento *proximo;


};
typedef struct _evento Evento;

Avaliação

A avaliação será realizada considerando a apresentação do código e as funcionalidades implementadas.
O trabalho pode ser realizado em dupla, porém, a avaliação considera não só o resultado final mas a participação e engajamento da equipe no desenvolvimento. Assim, os membros da dupla podem ter notas distintas.
Códigos que não sejam corretamente identados sofrerão duras penalidades
Reaproveitamento de código.
Criar funções reutilizáveis
A criatividade no desenvolvimento será recompensada.
Por exemplo, utilizar uma BST (binary search tree) para agilizar a busca dos dados (opcional)
Utilizar o conceito de TAD (.h e .c)
Será apreciado o trabalho que ordena os compromissos da agenda por data e hora.


