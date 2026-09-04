# INES.IA - Brazilian Institute for Software Engineering and Artificial Intelligence

Website oficial do **INES.IA** (*Brazilian Institute for Software Engineering and Artificial Intelligence*), uma rede nacional de pesquisa dedicada a impulsionar a ciência e a prática da Engenharia de Software na era da Inteligência Artificial.

---

## Sobre o Projeto

O **INES.IA** é liderado pelo Prof. Augusto Sampaio (UFPE) e reúne pesquisadores de todo o Brasil e parceiros internacionais para enfrentar os desafios mais urgentes na interseção entre a Engenharia de Software e a IA (*AI for SE & SE for AI*).

Este repositório contém o código-fonte da aplicação front-end do portal, desenvolvida com o gerador de sites estáticos **Hugo**.

---

## Pré-requisitos

Para executar o projeto localmente, você precisa ter o **Hugo** (preferencialmente a versão *Extended*) instalado em sua máquina.

### Instalação do Hugo 

```bash
# Recomendado: Instalação via Snap (Versão Extended com suporte a Sass/SCSS)
sudo snap install hugo --channel=extended

# Verifique se a instalação foi bem-sucedida
hugo version
```

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
hugo server 
```


### 3. Acessar no navegador
Abra o navegador e acesse o endereço fornecido no terminal:
```text
http://localhost:1313/
```

Qualquer alteração feita nos arquivos dentro das pastas `content/`, `layouts/` ou `static/` atualizará automaticamente a página no navegador.

---

## Regras de Contribuição para Desenvolvedores

1. **Nunca edite arquivos dentro da pasta `public/`**: Ela é sobrescrita a cada nova compilação.
2. **Alterações de Estrutura/HTML**: Modifique os arquivos dentro do diretório `layouts/`.
3. **Novas Imagens ou Favicons**: Adicione-os na pasta `static/` ou `static/img/`.