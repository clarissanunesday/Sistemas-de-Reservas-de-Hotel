# Sistema de Gerenciamento de Hotel

Este projeto é um sistema de gerenciamento de hotel que permite o cadastro de hóspedes, quartos e reservas. O sistema oferece funcionalidades para registrar, consultar e manipular informações sobre hóspedes e suas reservas.

## Funcionalidades

- **Gestão de Hóspedes**: Cadastro de hóspedes com informações como nome, telefone e e-mail.
- **Gestão de Quartos**: Registro de quartos disponíveis, incluindo número, tipo e preço.
- **Gestão de Reservas**: Registro de reservas feitas por hóspedes, relacionando hóspedes aos quartos reservados.
- **Consultas Avançadas**: Consultas para visualizar hóspedes com suas reservas e quartos disponíveis.

## Estrutura do Banco de Dados

### Tabelas

- **Hospedes**:
  - `id_hospede`: Identificador único do hóspede.
  - `nome`: Nome completo do hóspede.
  - `telefone`: Telefone de contato do hóspede.
  - `email`: E-mail do hóspede (único).

- **Quartos**:
  - `id_quarto`: Identificador único do quarto.
  - `numero`: Número do quarto (único).
  - `tipo`: Tipo do quarto (Simples, Duplo, Luxo, etc.).
  - `preco`: Preço por noite do quarto.

- **Reservas**:
  - `id_reserva`: Identificador único da reserva.
  - `id_hospede`: Referência ao hóspede que fez a reserva.
  - `id_quarto`: Referência ao quarto reservado.
  - `data_checkin`: Data de entrada do hóspede.
  - `data_checkout`: Data de saída do hóspede.

## Consultas e Operações Disponíveis

### Consultas

1. **Listar todos os hóspedes com suas reservas**:
   - Exibe todos os hóspedes registrados com suas informações e detalhes da reserva.

2. **Listar todos os quartos disponíveis para um determinado período**:
   - Exibe os quartos disponíveis para as datas solicitadas, permitindo verificar a disponibilidade.

### Atualizações e Deleções

1. **Atualizar informações de contato de um hóspede**:
   - Permite atualizar as informações de contato de um hóspede específico.

2. **Atualizar o preço de um quarto**:
   - Permite atualizar o preço de um quarto existente.

3. **Excluir um hóspede**:
   - Permite excluir um hóspede do sistema.

4. **Excluir uma reserva**:
   - Permite excluir uma reserva específica.

## Como Usar

1. **Criar o Banco de Dados**:
   Execute o script SQL fornecido para criar o banco de dados e suas respectivas tabelas.

2. **Inserir Dados**:
   Insira dados de hóspedes, quartos e reservas conforme necessário.

3. **Consultar e Manipular Dados**:
   Utilize as consultas SQL fornecidas para visualizar e modificar os dados.

## Licença

Este projeto está licenciado sob a Licença MIT. Consulte o arquivo `LICENSE` para mais detalhes.

## Requisitos

- MySQL ou outro sistema de gerenciamento de banco de dados compatível com SQL.
- Ferramenta para execução de scripts SQL, como MySQL Workbench ou phpMyAdmin.
