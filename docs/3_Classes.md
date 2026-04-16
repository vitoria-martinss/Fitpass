# ***Aluno***
### RF01, RF04, RF05, RF06, RF10
- idAluno
- nome
- cpf
- email
- telefone
- endereco
- rfid
- status
### Métodos Aluno
- Contratarplano()
- AgendarAula()
- CancelarAgeamento()
- AtualizarStatus()
- RegistrarAcesso()
- ReceberNotificacao()

# ***Plano***
### RF01, RF02, RF04
- idPlano
- nome
- tipo
- valor
- ativo
### Método Plano
- Ativar()
- Desativar()
- AlterarValor()

# ***Pagamento***
### RF03, RF04, RF09
- idPagamento
- data
- valor
- formaPagamento
- status
### Método Pagamento
- Registrar()
- Cancelar()
- Confirmar()

# ***Acesso***
### RF05, RF09
- idAcesso
- dataHora
- autorizado
### Método Acesso
- Registrar()
- Autorizar()
- Negar()

# ***Aula***
### RF06, RF07, RF09
- idAula
- nome
- horario
- capacidadeMaxima
### Método Aula
- contratarplano()
- AgendarAula()
- CancelarAgeamento()
- AtualizarStatus()
- RegistrarAcesso()
- ReceberNotificacao()

# ***Agendamento***
### RF06, RF10
- idAgendamento
- dataReserva
- status
### Método Agendamento
- Confirmar()
- Cancelar()

# ***Presenca***
### RF07
- idPresenca
- data
- presente
### Método Presenca
- Registrar()
- Cancelar()

# ***AvaliacaoFisica***
### RF08, RF10
- idAvaliacao
- data
- peso
- imc
- percentualGordura
- observacoes
- anexo
### Método Avaliacao
- Registrar()
- AtualizarDados()
- AnexarArquivos()

# ***Notificacao***
### RF10
- idNotificacao
- tipo
- dataEnvio
- status
- mensagem
### Método Notificacao
- Enviar()
- Marcarcomolida()

# ***Instrutor***
### RF07, RF08
- idInstrutor
- nome
- especialidade
### Método Instrutor
- RegistrarPresenca()
- RealizarAvaliacaoFisica()

# ***Recepcionista***
### RF01, RF03
- idRecepcionista
- nome
### Método Recepcionista
- CadastrarAluno()
- RegistrarPagamento

# ***Gerente***
### RF02, RF09
- idGerente
- nome
### Método Gerente
- GerenciarPlanos()
- EmitirRelatorios()
