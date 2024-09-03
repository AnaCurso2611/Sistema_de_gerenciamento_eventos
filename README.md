O sistema será utilizado para planejar e coordenar eventos, facilitando a inscrição de participantes e o gerenciamento das informações associadas. O banco de dados deve armazenar dados relevantes sobre os eventos e os participantes, e permitir consultas detalhadas e relatórios.

Funcionalidades Principais:

Gerenciamento de Eventos:

Cadastro de Eventos: Permitir a criação de eventos com informações detalhadas como nome, data, local e descrição.
Atualização de Eventos: Permitir a modificação das informações de eventos existentes.
Exclusão de Eventos: Permitir a remoção de eventos que já passaram ou que não são mais necessários.
Gerenciamento de Participantes:

Cadastro de Participantes: Permitir a adição de participantes com dados como nome, e-mail e telefone.
Atualização de Participantes: Permitir a atualização das informações de contato dos participantes.
Exclusão de Participantes: Permitir a remoção de participantes, se necessário.
Gerenciamento de Inscrições:

Registro de Inscrições: Permitir que participantes se inscrevam em eventos.
Consulta de Inscrições: Consultar quais participantes estão inscritos em eventos específicos e quais eventos um participante está inscrito.
Cancelamento de Inscrições: Permitir a exclusão de inscrições para eventos específicos.
Relatórios e Consultas:

Consultar Todos os Eventos: Obter uma lista completa de eventos disponíveis no sistema.
Participantes Inscritos em Evento: Consultar todos os participantes inscritos em um evento específico.
Eventos por Participante: Consultar todos os eventos em que um determinado participante está inscrito.
Participantes com Múltiplas Inscrições: Identificar participantes que estão inscritos em mais de um evento.
Requisitos Técnicos:

Banco de Dados: MySQL ou equivalente.
Estrutura do Banco de Dados: O banco de dados deve incluir as seguintes tabelas:
eventos: Para armazenar informações sobre eventos.
participantes: Para armazenar informações sobre participantes.
inscricoes: Para registrar a inscrição de participantes em eventos.
Scripts SQL:

Criação do Banco de Dados e Tabelas: Scripts para criar a estrutura do banco de dados e definir as tabelas e relacionamentos necessários.
Inserção de Dados: Scripts para adicionar dados de exemplo para eventos, participantes e inscrições.
Consultas e Relatórios: Scripts para consultar e gerar relatórios sobre eventos e inscrições.
Atualizações e Exclusões: Scripts para atualizar informações e excluir dados conforme necessário.
Instruções de Uso:

Execute os scripts SQL fornecidos para configurar o banco de dados e criar as tabelas.
Insira dados de exemplo usando os scripts de inserção.
Utilize os scripts de consulta para gerar relatórios e obter informações sobre eventos e inscrições.
Atualize e exclua dados conforme necessário para manter o sistema atualizado.
Objetivos do Projeto:

Facilitar a administração e o gerenciamento de eventos e inscrições.
Proporcionar uma visão clara e acessível das inscrições e eventos para melhor coordenação.
Garantir a integridade e a consistência dos dados relacionados a eventos e participantes.
Entrega:

O projeto será considerado concluído quando o banco de dados estiver configurado corretamente, os dados de exemplo forem inseridos e as consultas e relatórios estiverem funcionando conforme esperado.

# Sistema de Gerenciamento de Eventos

Este repositório contém o código SQL para criar e gerenciar um sistema de eventos. O sistema permite criar e gerenciar eventos, participantes e suas inscrições, bem como gerar relatórios úteis sobre as inscrições.

## Estrutura do Banco de Dados

O banco de dados `Sistema_eventos` possui as seguintes tabelas:

- **eventos**: Armazena informações sobre eventos.
  - `eventoID`: Identificador único do evento.
  - `nome`: Nome do evento.
  - `data`: Data do evento.
  - `local`: Local onde o evento será realizado.
  - `descricao`: Descrição do evento.

- **participantes**: Armazena informações sobre os participantes.
  - `participanteID`: Identificador único do participante.
  - `nome`: Nome do participante.
  - `email`: E-mail do participante.
  - `telefone`: Telefone do participante.

- **inscricoes**: Armazena informações sobre as inscrições dos participantes em eventos.
  - `inscricaoID`: Identificador único da inscrição.
  - `eventoID`: Referência ao evento em que o participante está inscrito.
  - `participanteID`: Referência ao participante que está inscrito.
  - `data_inscricao`: Data em que a inscrição foi realizada.

## Scripts SQL

### Criação do Banco de Dados e Tabelas

Os scripts para criar o banco de dados, tabelas e relacionamentos estão no início do arquivo.

### Inserção de Dados

Scripts para inserir dados de exemplo nas tabelas de eventos, participantes e inscrições.

### Consultas e Relatórios

Scripts para consultar eventos disponíveis, listar participantes inscritos em eventos, e identificar participantes que se inscreveram em múltiplos eventos.

### Atualizações e Exclusões

Scripts para atualizar informações de eventos e participantes, e para deletar eventos passados e inscrições de eventos específicos.

## Uso

1. Execute os scripts SQL em um servidor MySQL para criar o banco de dados e as tabelas.
2. Utilize as instruções de inserção para adicionar dados de exemplo.
3. Execute as consultas para gerar relatórios conforme necessário.
4. Use as instruções de atualização e exclusão para manter o banco de dados atualizado.

## Contribuições

Sinta-se à vontade para contribuir com melhorias ou sugestões para o sistema. Envie pull requests ou abra issues para discussões.

## Licença

Este projeto está licenciado sob a [Licença MIT](LICENSE).
