# Padrão de Commits e versionamento semântico

## Versionamento Semântico
### Dado um número de versão MAJOR.MINOR.PATCH, incremente:

1. versão Maior(MAJOR): quando fizer mudanças incompatíveis na API,
2. versão Menor(MINOR): quando adicionar funcionalidades mantendo compatibilidade,
3. versão de Correção(PATCH): quando corrigir falhas mantendo compatibilidade.

**fix**: um commit do tipo fix corrige um bug em sua base de código (isso se correlaciona com PATCH do Versionamento Semântico).

**feat**: um commit do tipo feat introduz um novo recurso na base de código (isso se correlaciona com MINOR Versionamento Semântico).

**BREAKING CHANGE**: um commit que possui um footer BREAKING CHANGE:, ou anexa um ! após o tipo/escopo, introduz uma alteração significativa na API (correlacionada com MAJOR Versionamento Semântico). Uma BREAKING CHANGE pode fazer parte de commits de qualquer tipo .

```
#Exemplo versionamento semântico:
Major.Minor.Patch -> v1.0.0
```

## Modelo
```git
<type>(<scope>): <subject>
<BLANK LINE>
<body>
<BLANK LINE>
<footer>
```

## Tipo
### Deve ser um dos seguintes:

**build**: alterações que afetam o sistema de compilação ou dependências externas.

**ci**: alterações em nossos arquivos e scripts de configuração de CI.

**docs**: Apenas a documentação muda.

**feat**: Um novo recurso.

**fix**: uma correção de bug.

**perf**: uma alteração de código que melhora o desempenho.

**refactor**: uma alteração de código que não corrige um bug nem adiciona um recurso.

**style**: Alterações que não afetam o significado do código (espaço em branco, formatação, falta de ponto e vírgula, etc.).

**test**: Adicionando testes ausentes ou corrigindo testes existentes.

```git
#Exemplo commits:
feat: criado botão enviar na homepage
```