# INES.IA - Brazilian Institute for Software Engineering and Artificial Intelligence

Website oficial do **INES.IA** (*Brazilian Institute for Software Engineering and Artificial Intelligence*), uma rede nacional de pesquisa dedicada a impulsionar a ciência e a prática da Engenharia de Software na era da Inteligência Artificial.

---

## Sobre o Projeto

O **INES.IA** é liderado pelo Prof. Augusto Sampaio (UFPE) e reúne pesquisadores de todo o Brasil e parceiros internacionais para enfrentar os desafios mais urgentes na interseção entre a Engenharia de Software e a IA (*AI for SE & SE for AI*).

Este repositório contém o código-fonte da aplicação front-end do portal, desenvolvida com o gerador de sites estáticos **Hugo**.

---

## Pré-requisitos

Para executar o projeto localmente, você precisa ter o **Hugo Extended** instalado em sua máquina. O deploy usa a versão **0.160.1** (veja `.github/workflows/deploy.yml`) — use a mesma localmente para evitar diferenças entre o seu build e o publicado.

### Instalação do Hugo

```bash
# macOS (Homebrew)
brew install hugo

# Linux (Snap) — a versão extended tem suporte a Sass/SCSS
sudo snap install hugo --channel=extended

# Verifique a instalação: a saída deve conter "extended"
hugo version
```

Em outras plataformas, ou para fixar exatamente a versão do deploy, baixe o binário `hugo_extended` correspondente em https://github.com/gohugoio/hugo/releases.

---

## Passo a Passo: Como Executar a Aplicação

Siga as instruções abaixo para rodar o servidor de desenvolvimento em seu ambiente local:

### 1. Clonar o repositório
```bash
git clone https://github.com/ines4ia/ines4ia.github.io
cd ines4ia.github.io
```

### 2. Iniciar o servidor de desenvolvimento
Execute o comando do Hugo para subir o servidor local com recarregamento em tempo real (*Live Reload*):

```bash
hugo server -D
```

A flag `-D` inclui os conteúdos marcados como rascunho (`draft: true`), que não aparecem no site publicado.


### 3. Acessar no navegador
Abra o navegador e acesse o endereço fornecido no terminal:
```text
http://localhost:1313/
```

Qualquer alteração feita nos arquivos dentro das pastas `content/`, `data/`, `layouts/`, `assets/` ou `static/` atualizará automaticamente a página no navegador.

---

## Regras de Contribuição para Desenvolvedores

1. **Nunca edite arquivos dentro da pasta `public/`**: Ela é sobrescrita a cada nova compilação.
2. **Alterações de Estrutura/HTML**: Modifique os arquivos dentro do diretório `layouts/`.
3. **Novas Imagens ou Favicons**: Adicione-os na pasta `static/` ou `static/img/`.
4. **Estilos**: O CSS fica em `assets/css/main.css` e é processado pelo Hugo Pipes. Prefira os tokens já definidos no topo do arquivo (`--brand`, `--bg-surface`, `--text-dark-muted`, `--nav-h`) a valores fixos, para manter a identidade visual e o contraste.
5. **Conteúdo estruturado**: Equipe, temas de pesquisa, teses, ferramentas e publicações vivem em `data/*.yaml`, não em `content/`.
6. **Nunca edite `data/publications.yaml` à mão**: ele é gerado. Edite `bibliography/publications.bib` e rode:
   ```bash
   python3 scripts/bib_to_yaml.py
   ```
7. **Antes de abrir um PR**, rode o build de produção para garantir que os templates não quebraram:
   ```bash
   hugo --gc --minify -D
   ```

### Publicando conteúdo novo

Novas publicações, teses, ferramentas, notícias e bios são solicitadas por **issue**, usando os templates em `.github/ISSUE_TEMPLATE/`. Cada tipo tem seu destino: teses em `data/theses.yaml`, ferramentas em `data/tools.yaml`, publicações em `bibliography/publications.bib` e bios em `data/team.yaml`.