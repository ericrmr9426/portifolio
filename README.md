# 👨‍💻 Portifólio Profissional — Eric Rodrigues

## 1. Explicação do funcionamento do projeto

O projeto consiste em um portfólio profissional desenvolvido com HTML5, CSS3 e Bootstrap 5.3.3, com o objetivo de apresentar perfil, formação acadêmica, habilidades, projetos e informações de contato.

A navegação é organizada em seções acessíveis por meio de um menu superior fixo (*navbar*), permitindo que o visitante encontre facilmente cada conteúdo.

A página conta com:
- **Menu de navegação:** acesso às seções Perfil, Projetos, Contatos, Formação e Habilidades.
- **Carrossel central:** apresentação visual de três conceitos principais, com navegação entre os banners.
- **Perfil profissional:** apresentação pessoal, objetivos e área de interesse.
- **Tecnologias e ferramentas:** identificação dos conhecimentos técnicos.
- **Projetos:** exposição de atividades e aplicações desenvolvidas.
- **Formação e habilidades:** apresentação da trajetória acadêmica e competências.
- **Contato:** acesso ao e-mail e perfil no GitHub.

O layout utiliza o sistema responsivo do Bootstrap, complementado por regras próprias de CSS para adaptar elementos, imagens e tipografia a diferentes tamanhos de tela.

## 2. 🎯 Descrição do recurso novo adicionado — Banner Central com Dropdown

O principal recurso novo implementado foi o **Banner Central com Dropdown**, integrado ao carrossel da página inicial.

O componente apresenta três banners independentes, identificados pelos conceitos:

- ✨ **Criatividade:** capacidade de transformar ideias em possibilidades.
- 🔎 **Análise:** capacidade de observar, investigar e compreender situações.
- 🚀 **Entrega:** dedicação e comprometimento na transformação de ideias em resultados.

Cada banner possui um botão centralizado que permite expandir ou recolher uma descrição textual relacionada ao conceito apresentado.

O recurso proporciona uma experiência interativa, permitindo que o visitante explore o significado de cada palavra sem precisar sair da página ou acessar outra seção.

Além da função informativa, os banners estabelecem uma identidade visual para o portfólio, representando três aspectos complementares do processo de desenvolvimento: **criar, compreender e realizar.**

## 3. ⚙️ Explicação de como o recurso foi implementado

A implementação utiliza recursos nativos do Bootstrap 5.3.3, combinando os componentes Carousel e Collapse.

### HTML5 — Estrutura

O carrossel foi construído utilizando as classes:
- `carousel`: define o componente de carrossel.
- `carousel-inner`: agrupa os slides.
- `carousel-item`: representa cada banner individual.
- `carousel-caption-custom`: classe personalizada para posicionar o conteúdo centralizado.

Cada banner possui um botão com os atributos `data-bs-toggle="collapse"` e `data-bs-target`, responsáveis por ativar a expansão e o recolhimento da descrição correspondente.

Exemplo de implementação:

```html
<button
  type="button"
  data-bs-toggle="collapse"
  data-bs-target="#descCriatividade"
  aria-expanded="false">

  <span>Criatividade</span>
  <span>▾</span>
</button>

<div class="collapse" id="descCriatividade">
  <div class="caption-desc-text">
    <p class="seu-texto">
      Descrição do conceito de criatividade.
    </p>
  </div>
</div>
```

Cada botão possui um identificador de destino exclusivo (`data-bs-target`), relacionado ao ID da respectiva descrição. Dessa forma, cada banner controla seu próprio conteúdo.

### CSS3 — Estilização e posicionamento

O CSS personalizado foi utilizado para posicionar o conteúdo no centro das imagens, utilizando:

- `position: absolute`: permite posicionar o banner sobre a imagem.
- `top: 50%` e `left: 50%`: definem o posicionamento central.
- `transform: translate(-50%, -50%)`: ajusta o elemento para centralização precisa.
- `object-fit: cover`: permite que as imagens preencham o espaço disponível sem distorção.
- `border-radius`: aplica o arredondamento dos cantos.
- `box-shadow`: adiciona profundidade ao elemento.

Também foi implementada uma regra de responsividade com `@media`, reduzindo o tamanho da fonte das descrições de 18px para 14px em telas com largura de até 768px.

### Bootstrap 5.3.3 — Interatividade

O Bootstrap é responsável pelo funcionamento dos recursos interativos.

O componente **Carousel** permite alternar entre os três banners, enquanto o componente **Collapse** controla a exibição das descrições.

A biblioteca JavaScript do Bootstrap é carregada ao final do documento HTML:

```html
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
```

Dessa maneira, não foi necessário desenvolver funções JavaScript próprias para controlar a abertura e o fechamento das descrições.

## 4. 🎨 Escolha das cores e identidade visual

A identidade visual foi construída a partir de uma combinação de cores que busca transmitir profissionalismo, clareza e criatividade.

| Cor | Código | Aplicação |
|---|---|---|
| Azul petróleo | `#176585` | Títulos, menu, botões e destaques |
| Verde suave | `#C2E4CB` | Fundo dos banners centrais |
| Branco | `#FFFFFF` | Áreas de conteúdo e contraste |
| Cinza claro | `#F8F9FA` | Fundo de seções |
| Cinza escuro | `#212529` | Rodapé |

A escolha do azul petróleo como cor principal estabelece unidade visual, enquanto o verde suave cria contraste com os elementos centrais, valorizando os três conceitos apresentados.

## 5. 🛠️ Tecnologias utilizadas

- <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg" width="18" height="18" /> **HTML5:** estruturação dos elementos e conteúdos.
- <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-original.svg" width="18" height="18" /> **CSS3:** estilização, posicionamento e responsividade.
- **Bootstrap 5.3.3:** componentes visuais, sistema de grid, Carousel e Collapse.
- **Google Fonts:** utilização da tipografia Plus Jakarta Sans.
- **Devicon:** biblioteca de ícones das tecnologias.

## 6. 📱 Responsividade

O projeto utiliza o sistema de grid do Bootstrap para adaptar a organização dos conteúdos a diferentes resoluções.

Foram adicionados ajustes específicos em CSS para controlar dimensões, posicionamento e tamanho das fontes, especialmente nos banners centrais.

O objetivo é preservar a legibilidade e a experiência de navegação tanto em computadores quanto em dispositivos móveis.

---

**Desenvolvido por Eric Rodrigues — 2026**  
*Portfólio acadêmico | Desenvolvimento de Sistemas*
