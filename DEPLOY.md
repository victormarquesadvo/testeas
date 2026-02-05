# Guia de Deploy - GitHub Pages

Este guia mostra como fazer deploy do site Aluguel de Sonhos no GitHub Pages.

## Pré-requisitos

- Git instalado no seu computador
- Conta no GitHub (https://github.com)

## Passo 1: Preparar o Repositório Local

Abra o terminal na pasta do projeto e execute:

```bash
# Inicializar repositório Git
git init

# Adicionar todos os arquivos
git add .

# Fazer o primeiro commit
git commit -m "Initial commit - Aluguel de Sonhos website"
```

## Passo 2: Repositório já Criado ✅

Você já tem o repositório criado em:
**https://github.com/victormarquesadvo/testeas**

## Passo 3: Conectar e Fazer Push

Execute os seguintes comandos:

```bash
# Adicionar repositório remoto
git remote add origin https://github.com/victormarquesadvo/testeas.git

# Renomear branch para main
git branch -M main

# Fazer push para GitHub
git push -u origin main
```

## Passo 4: Ativar GitHub Pages

1. No seu repositório no GitHub, vá em **Settings** (Configurações)
2. No menu lateral, clique em **Pages**
3. Em **Source**, selecione:
   - Branch: **main**
   - Folder: **/ (root)**
4. Clique em **Save**
5. Aguarde alguns minutos

## Passo 5: Acessar Seu Site

Após alguns minutos, seu site estará disponível em:
```
https://victormarquesadvo.github.io/testeas/
```

O GitHub Pages mostrará a URL exata na seção Pages.

## Atualizações Futuras

Quando fizer alterações no site:

```bash
# Adicionar mudanças
git add .

# Criar commit
git commit -m "Descrição das mudanças"

# Enviar para GitHub
git push
```

O site será atualizado automaticamente em alguns minutos!

## Solução de Problemas

### Arquivos não necessários (.gitignore)

Crie um arquivo `.gitignore` na raiz do projeto:

```
home.html
images.txt
.DS_Store
node_modules/
```

### Links relativos

Certifique-se de que todos os links internos usam caminhos relativos:
- ✅ `href="sobre.html"` 
- ✅ `href="css/style.css"`
- ❌ `href="/sobre.html"` (pode não funcionar)

### Domínio Personalizado (Opcional)

Se quiser usar um domínio próprio (ex: `alugueldesonhos.com.br`):

1. Vá em **Settings** → **Pages** → **Custom domain**
2. Digite seu domínio
3. Configure os DNS no seu registrador de domínios

## Recursos Úteis

- [Documentação GitHub Pages](https://docs.github.com/pt/pages)
- [Git Basics](https://git-scm.com/book/pt-br/v2)
