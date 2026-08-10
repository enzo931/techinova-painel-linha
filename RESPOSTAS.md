# Respostas do LAB 01

Nome: Enzo Manzoni Araújo
Matricula: 26174732
---

## M2 - Quem quebrou o painel

- **Hash curto do commit:** 01ef93b
- **Autor:** Tarcisio Melo <tarcisio.melo@techinova.com.br>
- **Data:** Mon Jun 15 22:38:00 2026 -0300
- **Linha alterada:**
  - **Antes (-):** `return (leitura - 32) * 5 / 9;`
  - **Depois (+):** `return leitura * 9 / 5 + 32;`
---

## M3 - O segredo vazado

**O que voce esperava ver no `git status` e o que apareceu:**

** Ao rodar o `git status`, o arquivo `config/credenciais.env` continuou sendo rastreado, mesmo que nós tenhamos criado um novo arquivo `.gitignore`, oque a primeira vista para mim foi estranho. Porém isso aconteceu porque o `.gitignore` só ignora arquivos novos. Como ele já havia sido commitado no passado, o Git continuou monitorando suas alterações até rodarmos o `git rm --cached`.

- **Pergunta obrigatória:** Depois desse push, alguém que clonar o repositório ainda consegue ler a chave?
- **Resposta:** Sim, qualquer pessoa que clonar o repositório ainda conseguirá ler a chave. Como ela foi commitada anteriormente, ela permanece registrada no histórico do Git e pode ser visualizada ao navegar pelos commits antigos.

---

## M4 - Colisao

**O que significavam os marcadores que apareceram dentro do arquivo:**

- `<<<<<<<` :
- `=======` :
- `>>>>>>>` :

**Qual pedaco veio de quem, e qual titulo voces decidiram manter:**

---

## Casa - Incidente na linha 3

**Hash do commit que quebrou o painel:**

**Hash do commit de revert:**

**Por que `git revert` e nao `git reset` neste caso:**
