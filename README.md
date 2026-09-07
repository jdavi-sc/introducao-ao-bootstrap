# Bootstrap — Introdução e Fundamentos

Repositório criado com o objetivo de estudar e praticar os principais conceitos e componentes do **Bootstrap**, explorando sua utilização na construção de interfaces web responsivas, organizadas e consistentes.

O projeto reúne exemplos práticos desenvolvidos durante os estudos, servindo como material de consulta para futuros projetos e como registro da evolução no aprendizado de desenvolvimento web.

---

## 📚 Sobre o projeto

O **Bootstrap** é um framework front-end utilizado para facilitar o desenvolvimento de interfaces web responsivas e mobile-first. Ele fornece uma coleção de classes CSS, componentes prontos e recursos JavaScript que permitem construir interfaces de maneira mais rápida e consistente.

Este repositório foi desenvolvido como um **ambiente de estudos**, no qual cada exemplo demonstra na prática a utilização de diferentes recursos oferecidos pelo Bootstrap.

A ideia é que o projeto possa ser consultado posteriormente para:

* Revisar conceitos aprendidos;
* Consultar classes e componentes;
* Reutilizar estruturas em projetos futuros;
* Entender como determinados componentes do Bootstrap são construídos;
* Praticar desenvolvimento de interfaces responsivas;
* Servir como material de apoio para outros estudantes.

---

## 🎯 Objetivos

Os principais objetivos deste repositório são:

* Compreender os fundamentos do Bootstrap;
* Aprender a utilizar suas classes utilitárias;
* Entender o sistema de grid;
* Trabalhar com containers responsivos;
* Explorar componentes pré-estilizados;
* Praticar a criação de interfaces responsivas;
* Compreender a utilização dos componentes JavaScript do Bootstrap;
* Criar uma base de consulta para projetos futuros.

---

## 🛠️ Tecnologias utilizadas

| Tecnologia      | Utilização                               |
| --------------- | ---------------------------------------- |
| **HTML5**       | Estrutura das páginas e exemplos         |
| **CSS3**        | Estilizações complementares              |
| **Bootstrap 5** | Framework utilizado nos exemplos         |
| **JavaScript**  | Funcionamento de componentes interativos |
| **Git**         | Controle de versão                       |
| **GitHub**      | Hospedagem do repositório                |

---

## 📖 Conteúdos estudados

O repositório aborda inicialmente os seguintes conceitos e componentes:

### 📦 Containers

Os containers são utilizados para organizar e limitar o conteúdo da página.

Foram estudados principalmente:

* `.container`
* `.container-fluid`

O `.container` possui larguras responsivas de acordo com o breakpoint, enquanto `.container-fluid` ocupa toda a largura disponível da viewport.

> Exemplo de aplicação: criação de áreas de conteúdo centralizadas e responsivas.

---

### 📝 Tipografia

O Bootstrap fornece classes e estilos pré-definidos para trabalhar com textos e elementos tipográficos.

Foram explorados conceitos como:

* Headings;
* Parágrafos;
* Alinhamento de texto;
* Pesos de fonte;
* Cores de texto;
* Tamanhos;
* Elementos de destaque.

Exemplos de classes:

```html
<h1>Título</h1>

<p class="text-center">
    Texto centralizado
</p>

<p class="fw-bold">
    Texto em negrito
</p>
```

---

### 🔘 Botões

O Bootstrap disponibiliza diversas classes para criação de botões padronizados.

Algumas das classes estudadas:

```html
<button class="btn btn-primary">
    Primary
</button>

<button class="btn btn-success">
    Success
</button>

<button class="btn btn-danger">
    Danger
</button>
```

Também podem ser utilizados diferentes tamanhos, estados e estilos de botão.

Principais variações:

* Primary
* Secondary
* Success
* Danger
* Warning
* Info
* Light
* Dark
* Link
* Outline

---

### 🧱 Grid System

O sistema de **Grid** é um dos principais recursos do Bootstrap para construção de layouts responsivos.

O sistema é baseado em:

```text
Container
   │
   └── Row
        │
        ├── Column
        ├── Column
        └── Column
```

Exemplo:

```html
<div class="container">
    <div class="row">

        <div class="col">
            Coluna 1
        </div>

        <div class="col">
            Coluna 2
        </div>

        <div class="col">
            Coluna 3
        </div>

    </div>
</div>
```

Também é possível definir diferentes comportamentos para diferentes tamanhos de tela:

```html
<div class="row">

    <div class="col-12 col-md-6 col-lg-4">
        Conteúdo
    </div>

    <div class="col-12 col-md-6 col-lg-4">
        Conteúdo
    </div>

    <div class="col-12 col-md-6 col-lg-4">
        Conteúdo
    </div>

</div>
```

Essa abordagem permite construir layouts que se adaptam a smartphones, tablets e desktops.

---

### 🧭 Navbar

A **Navbar** é utilizada para criar barras de navegação.

Exemplo de estrutura:

```html
<nav class="navbar navbar-expand-lg">
    <div class="container">

        <a class="navbar-brand" href="#">
            Logo
        </a>

        <div class="navbar-nav">
            <a class="nav-link" href="#">
                Home
            </a>

            <a class="nav-link" href="#">
                Sobre
            </a>

        </div>

    </div>
</nav>
```

Também foram explorados recursos como:

* Logo/Brand;
* Links;
* Navbar responsiva;
* Menu colapsável;
* Botão toggler;
* Cores;
* Alinhamento;
* Containers.

O Bootstrap permite transformar a navbar em um menu responsivo que pode ser expandido ou recolhido de acordo com o tamanho da tela.

---

### 🖼️ Carousel

O **Carousel** permite criar apresentações de conteúdo em formato de slideshow.

Entre suas possibilidades estão:

* Imagens;
* Indicadores;
* Botões de navegação;
* Transições;
* Reprodução automática.

Estrutura básica:

```html
<div id="carouselExample" class="carousel slide">

    <div class="carousel-inner">

        <div class="carousel-item active">
            Conteúdo 1
        </div>

        <div class="carousel-item">
            Conteúdo 2
        </div>

    </div>

</div>
```

O Bootstrap fornece classes específicas para estruturar o carousel e seus controles.

---

### 🪟 Modal

O **Modal** é utilizado para apresentar conteúdo sobreposto à página atual, sem precisar navegar para outra página.

Pode ser utilizado para:

* Mensagens;
* Formulários;
* Confirmações;
* Informações adicionais;
* Diálogos com o usuário.

Exemplo simplificado:

```html
<button
    type="button"
    class="btn btn-primary"
    data-bs-toggle="modal"
    data-bs-target="#exampleModal"
>
    Abrir Modal
</button>
```

O modal é controlado por atributos `data-bs-*` e pelos componentes JavaScript do Bootstrap.

---

## 📁 Estrutura do projeto

A estrutura atual do projeto segue uma organização simples, mantendo os exemplos separados do arquivo de documentação:

```text
introducao-ao-bootstrap/
│
├── examples/
│   │
│   ├── buttons/
│   ├── carousel/
│   ├── containers/
│   ├── grid/
│   ├── modal/
│   ├── navbar/
│   └── typography/
│
├── LICENSE
│
└── README.md
```

> **Observação:** caso novos exemplos sejam adicionados futuramente, recomenda-se manter cada conceito em seu próprio diretório dentro de `examples/`.

---

## 🚀 Como executar os exemplos

Como este projeto é composto principalmente por HTML, CSS e Bootstrap, não é necessário instalar dependências complexas para executar os exemplos.

### 1. Clone o repositório

```bash
git clone https://github.com/jdavi-sc/introducao-ao-bootstrap.git
```

### 2. Acesse o diretório

```bash
cd introducao-ao-bootstrap
```

### 3. Abra os exemplos

Entre na pasta:

```text
examples/
```

e abra o arquivo `index.html` ou o HTML correspondente ao exemplo que deseja estudar.

Também é possível utilizar uma extensão como **Live Server** no Visual Studio Code para executar os exemplos em um servidor local.

---

## 🌐 Como o Bootstrap é utilizado

O Bootstrap pode ser adicionado ao projeto de diferentes maneiras.

Uma das formas mais simples é utilizar o **CDN**.

### CSS

```html
<link
    href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.8/dist/css/bootstrap.min.css"
    rel="stylesheet"
>
```

### JavaScript

Para componentes interativos, como **Carousel** e **Modal**, também é necessário carregar o JavaScript do Bootstrap:

```html
<script
    src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.8/dist/js/bootstrap.bundle.min.js">
</script>
```

A utilização do JavaScript é necessária para determinados componentes interativos do Bootstrap.

---

## 📱 Responsividade

Um dos principais objetivos do Bootstrap é facilitar a criação de interfaces **responsivas**.

O framework adota uma abordagem **mobile-first**, permitindo que os elementos sejam configurados de acordo com diferentes breakpoints.

Exemplo:

```html
<div class="col-12 col-md-6 col-lg-4">
    Conteúdo
</div>
```

Nesse exemplo:

| Breakpoint | Comportamento           |
| ---------- | ----------------------- |
| `col-12`   | Ocupa toda a largura    |
| `col-md-6` | Ocupa metade da largura |
| `col-lg-4` | Ocupa 1/3 da largura    |

Isso permite que o mesmo layout se adapte a diferentes dispositivos sem a necessidade de criar uma página completamente diferente para cada resolução.

---

## 🧠 Conceitos importantes para estudar

Além de memorizar classes, este projeto tem como objetivo compreender **como e por que utilizar cada recurso**.

Durante os estudos, é interessante observar:

### Containers

```text
.container
.container-fluid
```

### Grid

```text
.container
.row
.col
.col-*
.col-sm-*
.col-md-*
.col-lg-*
.col-xl-*
.col-xxl-*
```

### Tipografia

```text
text-*
fw-*
fs-*
display-*
```

### Botões

```text
.btn
.btn-primary
.btn-secondary
.btn-success
.btn-danger
.btn-warning
.btn-info
.btn-dark
.btn-light
.btn-outline-*
```

### Navbar

```text
.navbar
.navbar-brand
.navbar-nav
.nav-link
.navbar-toggler
.navbar-collapse
```

### Carousel

```text
.carousel
.carousel-inner
.carousel-item
.carousel-control-prev
.carousel-control-next
.carousel-indicators
```

### Modal

```text
.modal
.modal-dialog
.modal-content
.modal-header
.modal-body
.modal-footer
```

---

## 📚 Fonte de estudo

O conteúdo deste repositório foi desenvolvido com base principalmente nos materiais de estudo disponibilizados pelo **W3Schools**, especialmente no tutorial de Bootstrap 5.

A documentação foi utilizada como **referência para aprendizado**, enquanto os exemplos deste repositório foram desenvolvidos com finalidade de prática e consolidação dos conhecimentos.

### Referência principal

**W3Schools — Bootstrap 5 Tutorial**

https://www.w3schools.com/bootstrap5/

O tutorial aborda conceitos fundamentais do Bootstrap, incluindo containers, grid, tipografia, botões, navbars, carousel, modal e diversos outros componentes.

---

## 📄 Licença

Este projeto está licenciado sob a **MIT License**.

Consulte o arquivo [`LICENSE`](./LICENSE) para obter mais informações.

---

## 👨‍💻 Autor

**José Davi**

Estudante de **Análise e Desenvolvimento de Sistemas**, interessado em desenvolvimento de software, desenvolvimento web e tecnologias relacionadas à programação.

### GitHub

[github.com/jdavi-sc](https://github.com/jdavi-sc)