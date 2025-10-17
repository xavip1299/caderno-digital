# Caderno Digital Acadêmico

Este é um caderno digital criado com Jekyll para GitHub Pages, destinado ao acompanhamento e documentação do percurso académico.

## 🚀 Como Começar

### Pré-requisitos
- Ruby (versão 2.5 ou superior)
- Bundler
- Git

### Instalação Local

1. **Clone o repositório**:
```bash
git clone https://github.com/seuusername/caderno-digital.git
cd caderno-digital
```

2. **Instale as dependências**:
```bash
bundle install
```

3. **Execute localmente**:
```bash
bundle exec jekyll serve
```

4. **Aceda ao site**:
Abra o browser em `http://localhost:4000`

### Deploy no GitHub Pages

1. **Crie um repositório no GitHub** com o nome `caderno-digital`

2. **Configure as GitHub Pages**:
   - Vá às Settings do repositório
   - Na secção Pages, selecione "Deploy from a branch"
   - Escolha a branch `main` e a pasta `/ (root)`

3. **Atualize o `_config.yml`**:
   - Altere `url` para `https://seuusername.github.io`
   - Altere `baseurl` para `/caderno-digital`

4. **Faça push do código**:
```bash
git add .
git commit -m "Configuração inicial do caderno digital"
git push origin main
```

## 📁 Estrutura do Projeto

```
caderno-digital/
├── _config.yml          # Configuração principal do Jekyll
├── _layouts/            # Templates HTML
├── _posts/              # Posts do blog
├── _sass/               # Estilos SCSS personalizados
├── assets/              # CSS, imagens, scripts
├── index.html           # Página inicial
├── sobre.md             # Página sobre
├── disciplinas.md       # Página de disciplinas
├── projetos.md          # Página de projetos
├── recursos.md          # Página de recursos
├── contato.md          # Página de contacto
├── Gemfile             # Dependências Ruby
└── README.md           # Este arquivo
```

## ✍️ Como Criar Conteúdo

### Novo Post

1. **Crie um arquivo** na pasta `_posts/` com o formato:
   `YYYY-MM-DD-titulo-do-post.md`

2. **Adicione o front matter**:
```yaml
---
layout: post
title: "Título do Post"
date: 2024-10-17 10:00:00 +0000
categories: [categoria1, categoria2]
tags: [tag1, tag2, tag3]
author: "Seu Nome"
---
```

3. **Escreva o conteúdo** em Markdown

### Nova Página

1. **Crie um arquivo** `.md` na raiz do projeto
2. **Adicione o front matter**:
```yaml
---
layout: page
title: "Título da Página"
permalink: /nome-da-pagina/
---
```

## 🎨 Personalização

### Configurações Principais
Edite o arquivo `_config.yml` para personalizar:
- Título e descrição do site
- Informações do autor
- URL do GitHub Pages
- Configurações de navegação

### Estilos Visuais
Os estilos personalizados estão em `_sass/_custom.scss`:
- Cores do tema
- Tipografia
- Layout e espaçamentos
- Responsividade

### Navegação
Para adicionar páginas ao menu principal, edite a secção `header_pages` no `_config.yml`:
```yaml
header_pages:
  - sobre.md
  - disciplinas.md
  - projetos.md
  - recursos.md
  - contato.md
  - nova-pagina.md
```

## 📝 Dicas de Conteúdo

### Estrutura Recomendada para Posts
1. **Contexto**: Situação ou aula que motivou o post
2. **Conceitos principais**: Definições e explicações
3. **Análise crítica**: Reflexões pessoais
4. **Aplicações práticas**: Exemplos concretos
5. **Questões futuras**: Pontos para explorar

### Uso de Tags e Categorias
- **Categorias**: Grandes áreas temáticas (máximo 2-3 por post)
- **Tags**: Tópicos específicos (múltiplas tags são bem-vindas)

### Formatação em Markdown
```markdown
# Título Principal
## Subtítulo
### Sub-subtítulo

**Texto em negrito**
*Texto em itálico*

- Lista com pontos
1. Lista numerada

[Link para página](URL)

> Citação em bloco

`código inline`

```código em bloco```
```

## 🔧 Manutenção

### Atualizações Regulares
- Revise periodicamente o `_config.yml`
- Atualize as dependências: `bundle update`
- Teste localmente antes de fazer push

### Backup
- Mantenha backups regulares do repositório
- Considere fazer fork como backup adicional

### SEO e Performance
- Use títulos descritivos
- Adicione meta descrições aos posts
- Otimize imagens antes de adicionar
- Use tags e categorias consistentemente

## 📚 Recursos Úteis

### Jekyll
- [Documentação oficial](https://jekyllrb.com/docs/)
- [GitHub Pages + Jekyll](https://docs.github.com/pt/pages/setting-up-a-github-pages-site-with-jekyll)

### Markdown
- [Guia de Markdown](https://www.markdownguide.org/)
- [Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)

### Design e UX
- [Minima Theme](https://github.com/jekyll/minima)
- [Jekyll Themes](https://jekyllthemes.io/)

## 🆘 Resolução de Problemas

### Problemas Comuns

**Jekyll não instala**:
```bash
gem install bundler jekyll
bundle install
```

**Site não atualiza no GitHub Pages**:
- Verifique se há erros na aba Actions do GitHub
- Confirme que o `_config.yml` está correto
- Aguarde alguns minutos para propagação

**Estilos não aparecem**:
- Verifique o `baseurl` no `_config.yml`
- Confirme que o arquivo `assets/css/style.scss` existe

### Logs e Debug
Para ver logs detalhados:
```bash
bundle exec jekyll serve --verbose
```

## 📄 Licença

Este projeto está sob licença MIT. Veja o arquivo LICENSE para mais detalhes.

## 🤝 Contribuições

Contribuições são bem-vindas! Por favor:
1. Faça fork do projeto
2. Crie uma branch para sua feature
3. Commit suas mudanças
4. Push para a branch
5. Abra um Pull Request

---

**Última atualização**: Outubro 2024

Para mais informações ou suporte, visite a página de [contacto](contato.md) do site.