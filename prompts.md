# Como este site foi construído

Este portfólio foi criado inteiramente via *vibe coding* em conversa com Claude (Anthropic), sem escrever uma linha de código manualmente. Abaixo está o recorte dos prompts que guiaram a construção, do briefing inicial ao resultado final.

---

### 1. Briefing inicial

```
utilizando vibe coding vamos criar um portfolio para um profissional de dados formado em design

o portfolio sera um site e vai conter descrição dos projetos, breve apresentação do profissional e formulario de contato

solicite os dados que voce precisa para começar
```

### 2. Extração de conteúdo a partir do LinkedIn

Em vez de digitar o currículo manualmente, o conteúdo foi extraído direto do perfil profissional:

```
Extraia as principais informações do linkedin: https://www.linkedin.com/in/ingrid-sabino/
```

> O LinkedIn bloqueia leitura automatizada, então o fallback foi exportar o perfil em PDF e enviar o arquivo diretamente no chat.

### 3. Direção de estilo (referência visual)

```
ajuste o estilo do site para fundo cinza e sem cor de destaque
utilize um estilo mais criativo / designer
foque em monotypes para caracteres especiais
e tipografias mais geometricas
troque o scroll por cards nas experiencias
exemplo/inspo: https://majd-portfolio.framer.website/
```

> Passar um link de referência real foi o que mais mudou a qualidade do resultado: em vez de descrever o estilo por adjetivos, a IA analisou o site e traduziu a lógica de composição (tipografia, ritmo, elementos monoespaçados) para o contexto do projeto.

### 4. Funcionalidade: seletor de idiomas

```
crie um botao que automaticamente troque a versão do site para ingles e espanhol
```

### 5. Nova seção + revisão de copy

```
troque a fonte principal pela DM Sans
inclua uma seção de serviços prestados:

* dados e analytics: consultoria de dados e insigths para empresas, construção de produtos de dados (automações, tabelas, dashboards e planilhas de acompanhamentos)
* design: diagramação de apresentações executivas e criação de sites

inlcua ícones/imagens na seção de serviços prestados

```

> Pedir explicitamente para remover "traços de copy feito com IA" (travessões em excesso, cadência repetitiva) foi um ajuste fino importante para o texto soar mais natural.

### 6. Refinamento final

```
retire a imagem abstrata
aumente o tamanho da fonte do nome e do trecho 'traduzindo complexidade em clareza'

na seção de idiomas troque ingles e espanhol para avançado ao inves de fluente
```

---

## O que aprendi sobre prompting nesse processo

- **Referências visuais valem mais que adjetivos.** Um link real ("quero algo parecido com isso") rende resultado muito mais preciso do que tentar descrever estilo em palavras.
- **Enviar arquivos reais** (PDF do LinkedIn, foto de um desenho) elimina retrabalho: a IA extrai e adapta o conteúdo em vez de você ter que redigitar tudo.
- **Iterar em camadas** (estrutura → estilo → conteúdo → funcionalidade → polimento) funcionou melhor do que tentar pedir tudo de uma vez.

---

*Site construído com HTML, CSS e JavaScript puro (sem framework), com tradução PT/EN/ES via JavaScript e formulário de contato integrado por mailto.*
