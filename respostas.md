# Módulo 02 — Padrões de Projeto — Prática

## 1. Mensagens de commit

**Enunciado:**

Para cada cenário abaixo, escreva a mensagem de commit correta (prefixo + descrição):

1. Você adicionou um botão de "esqueci minha senha" na tela de login.
2. Você corrigiu um erro que travava o cadastro quando o campo de e-mail estava vazio.
3. Você reorganizou as funções do módulo de autenticação sem mudar o comportamento.
4. Você atualizou o `README.md` explicando como rodar o projeto localmente.
5. Você configurou o pipeline de CI para rodar os testes automaticamente a cada push.

### Respostas

1. `feat: adiciona botão esqueci minha senha`
2. `fix: corrigi erro no cadastro com e-mail vazio`
3. `refactor: reorganiza funções do módulo de autenticação`
4. `docs: atualiza o README.md`
5. `ci: configura pipeline para executar testes a cada push`

---

## 2. Nomes de branch

**Enunciado:**

Renomeie as branches abaixo para o padrão `PREFIXO/TASK-NOME-DA-TAREFA` (invente um número de tarefa):

1. Uma branch para corrigir um erro crítico de autenticação em produção.
2. Uma branch para adicionar um cadastro de usuário.
3. Uma branch para adicionar testes ao módulo de pagamentos.

Depois, escreva o comando `git branch -m` que renomeia a branch atual para o nome corrigido.

### Respostas

1. `hotfix/1234-bug-autenticacao`

```bash
git branch -m hotfix/1234-bug-autenticacao
```

2. `feature/1456-cadastro-usuario`

```bash
git branch -m feature/1456-cadastro-usuario
```

3. `test/2357-testes-modulo-pagamentos`

```bash
git branch -m test/2357-testes-modulo-pagamentos
```

---

## 3. Versionamento semântico

**Enunciado:**

Dado que a versão atual do projeto é `2.3.1`, diga qual deve ser a próxima versão em cada caso, e por quê:

1. Você corrigiu um bug que não muda nenhuma interface pública.
2. Você adicionou um novo endpoint na API, sem alterar os existentes.
3. Você removeu um parâmetro obrigatório de uma função pública, quebrando quem já usava a versão anterior.

### Respostas

1. **`2.3.2`**

   Corrigiu um bug e manteve a compatibilidade com a versão anterior.

2. **`2.4.0`**

   Adiciona uma nova função, mantendo a compatibilidade com as funcionalidades existentes.

3. **`3.0.0`**

   Houve uma mudança sem compatibilidade com a versão anterior.

---

## 4. Tags

**Enunciado:**

Escreva os comandos para:

1. Criar uma tag anotada `v2.4.0` na branch `main`, com a mensagem `"Lançamento da versão 2.4.0"`.
2. Enviar essa tag ao repositório remoto.
3. Enviar todas as tags locais de uma vez.

### Respostas

1. Criar a tag anotada:

```bash
git tag -a v2.4.0 -m "Lançamento da versão 2.4.0"
```

2. Enviar a tag ao repositório remoto:

```bash
git push origin v2.4.0
```

3. Enviar todas as tags locais:

```bash
git push origin --tags
```

---

## 5. Pull Request

**Enunciado:**

Escreva um Pull Request completo (título + descrição, seguindo a estrutura da teoria) para a seguinte mudança:

> "Você criou a tela de recuperação de senha, motivada por reclamações de usuários que esqueciam a senha e não tinham como recuperar o acesso. A tela usa o mesmo componente de formulário já existente na tela de login."

### Resposta

**Título:**

> Adiciona tela de recuperação de senha

**Por que:**

> Usuários reclamavam que esqueciam a senha e não tinham como recuperar o acesso.

**Como foi feito:**

> Foi utilizado como referência o formulário já existente na tela de login.

**Responsável:**

> @KlismanAmiden
