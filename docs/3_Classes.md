***Aluno***
RF01, RF04, RF05, RF06, RF10
- idAluno
- nome
- cpf
- email
- telefone
- endereco
- rfid
- status

ContratarPlano()
AgendarAula()
CancelarAgendamento()
AtualizarStatus()
RegistrarAcesoo()
ReceberNotificacao()


***Plano***
RF01, RF02, RF04
- idPlano
- nome
- tipo
- valor
- ativo

Ativar()
Desativar()
AlterarValor()

***Pagamento***
RF03, RF04, RF09
- idPagamento
- data
- valor
- formaPagamento
- status

Registrar()
Confirmar()
Cancelar()

***Acesso***
RF05, RF09
- idAcesso
- dataHora
- autorizado

Registrar()
Autorizar()
Negar()

***Aula***
RF06, RF07, RF09
- idAula
- nome
- horario
- capacidadeMaxima

DisponibilidadeHorario()
ReservarVaga()
LiberarVaga()
RegistrarPresenca()

***Agendamento***
RF06, RF10
- idAgendamento
- dataReserva
- status

Confirmar()
Cancelar()

***Presenca***
RF07
- idPresenca
- data
- presente

Registrar()

***AvaliacaoFisica***
RF08, RF10
- idAvaliacao
- data
- peso
- imc
- percentualGordura
- observacoes
- anexo

Registrar()
AtualizarDados()
AnexarArquivo()

***Notificacao***
RF10
- idNotificacao
- tipo
- dataEnvio
- status
- mensagem

Enviar()
MarcarComoLida()

***Instrutor***
RF07, RF08
- idInstrutor
- nome
- especialidade

RegistrarPresenca()
RealizarAvalicaoFisica()

***Recepcionista***
RF01, RF03
- idRecepcionista
- nome

CadastrarAluno()
RegistrarPagamento()

***Gerente***
RF02, RF09
- idGerente
- nome

GerenciarPlanos()
