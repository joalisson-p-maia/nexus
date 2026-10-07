### Nexus

### Introdução

Nexus é uma aplicação para ajudar os estudantes e professores a manterem os horários escolares em dia, ou seja, atualizados, para que ambas as partes fiquem cientes dos horários e dias de aula.

---

### Padrões de Branch

Aqui na Nexus pode seguir os padrões de branch abaixo:

| Padrão | Significado |
|---|---|
| `feat/atividadeFeita` | **feat** = Funcionalidade nova |
| `refactor/atividadeFeita` | **refactor** = Atualizando funcionalidade |
| `docs/atividadeFeita` | **docs** = Criando ou atualizando arquivos de documentação |
| `test/atividadeFeita` | **test** = Enviando testes de funcionalidade |
| `chore/atividadeFeita` | **chore** = Usado para arquivos de configuração |
| `fix/atividadeFeita` | **fix** = Corrigindo bug |

---

### Padrões de Commit

Aqui na Nexus pode seguir os padrões de commit abaixo:

| Padrão | Significado |
|---|---|
| `(feat): atividadeFeita` | **feat** = Funcionalidade nova |
| `(refactor): atividadeFeita` | **refactor** = Atualizando funcionalidade |
| `(docs): atividadeFeita` | **docs** = Criando ou atualizando arquivos de documentação |
| `(test): atividadeFeita` | **test** = Enviando testes de funcionalidade |
| `(chore): atividadeFeita` | **chore** = Usado para arquivos de configuração |
| `(fix): atividadeFeita` | **fix** = Corrigindo bug |

---

### Padrões de Pull Request

Os Pull Requests da Nexus devem seguir um padrão para facilitar a revisão, organização e entendimento das alterações realizadas pela equipe.

### Título do Pull Request

O título deve seguir o mesmo padrão utilizado nos commits:

````
(tipo): descrição da atividade
````

Onde `tipo` pode ser:

- **feat** = Nova funcionalidade
- **refactor** = Atualização ou melhoria de uma funcionalidade existente
- **docs** = Criação ou atualização de documentação
- **test** = Criação ou atualização de testes
- **chore** = Configurações, dependências ou tarefas administrativas
- **fix** = Correção de bug

### Exemplos

- `(feat): adiciona cadastro de professores`
- `(feat): implementa gerenciamento de horários`
- `(refactor): reorganiza serviço de autenticação`
- `(fix): corrige atualização do horário da turma`
- `(test): adiciona testes para cadastro de disciplinas`
- `(docs): atualiza documentação da API`
- `(chore): atualiza dependências do projeto`

O título deve ser curto, objetivo e descrever o que foi realizado, evitando descrições genéricas como:

- `(feat): alterações`
- `(fix): correções`
- `(refactor): mudanças no código`

### Checklist do Pull Request

Antes de abrir um Pull Request, o responsável deve verificar os seguintes itens:

### Código

- [ ] A implementação segue os padrões definidos pelo projeto.
- [ ] O código está organizado e legível.
- [ ] Não existem códigos desnecessários ou comentados.
- [ ] Não foram adicionadas credenciais, tokens ou informações sensíveis.
- [ ] A alteração não quebra funcionalidades existentes.

### Testes

- [ ] Foram realizados testes da funcionalidade alterada.
- [ ] Foram adicionados ou atualizados testes automatizados quando necessário.
- [ ] Os testes existentes continuam passando.
- [ ] Foram verificados cenários de erro e casos extremos quando aplicável.

### Banco de Dados

- [ ] As alterações no banco de dados possuem migration quando necessário.
- [ ] As migrations foram testadas.
- [ ] Não foram adicionados dados sensíveis desnecessariamente.
- [ ] Relacionamentos e restrições estão de acordo com o modelo do sistema.

### Documentação

- [ ] A documentação foi atualizada quando necessário.
- [ ] Novos endpoints, funcionalidades ou regras foram documentados.
- [ ] Alterações que afetam a utilização do sistema foram descritas no PR.

### Pull Request

- [ ] O título segue o padrão definido pela Nexus.
- [ ] A descrição explica claramente o que foi alterado.
- [ ] O PR possui contexto suficiente para ser revisado por outro membro da equipe.
- [ ] O PR está relacionado à issue/tarefa correspondente, quando existir.
- [ ] Foram anexadas imagens, vídeos ou exemplos quando a alteração possui impacto visual ou comportamental.

### Descrição do Pull Request

A descrição deve apresentar, de forma objetiva, o que foi desenvolvido e por quê.

Utilize o modelo abaixo:

````markdown
## Descrição

Descreva brevemente o que foi desenvolvido ou corrigido.

## Motivação

Explique o motivo da alteração e qual problema ela resolve.

## Alterações realizadas

- Alteração 1
- Alteração 2
- Alteração 3

## Testes realizados

- Teste 1
- Teste 2
- Teste 3

### Evidências

Adicione imagens, vídeos, prints ou exemplos quando necessário.

### Checklist

- [ ] Código revisado
- [ ] Testes realizados
- [ ] Documentação atualizada, quando necessário
- [ ] Sem dados sensíveis
- [ ] Sem conflitos com a branch principal
````

### Fluxo de Pull Request

O fluxo recomendado para a Nexus é:

````
Branch de desenvolvimento
        ↓
Implementação
        ↓
Commit
        ↓
Push
        ↓
Pull Request
        ↓
Revisão de código
        ↓
Correções, se necessário
        ↓
Aprovação
        ↓
Merge
````

O Pull Request deve ser criado somente quando a alteração estiver pronta para revisão.

Caso sejam necessárias alterações após a revisão, elas devem ser realizadas na mesma branch do Pull Request.

### Revisão de Pull Request

O responsável pela revisão deve verificar:

- A implementação atende ao objetivo da tarefa.
- O código segue os padrões do projeto.
- Não existem problemas evidentes de segurança.
- Não existem alterações desnecessárias.
- Os testes são suficientes para a alteração.
- A alteração não quebra funcionalidades existentes.
- A estrutura utilizada está adequada ao projeto.

Após a revisão, o Pull Request pode ser:

- **Aprovado:** quando estiver pronto para merge.
- **Alterações solicitadas:** quando forem necessárias correções antes do merge.
- **Rejeitado/fechado:** quando a abordagem não for adequada ou a alteração não for mais necessária.