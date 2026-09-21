# 💈 PD Barber

Projeto desenvolvido para a atividade da **Barbearia PD**, com foco na criação de uma interface responsiva para uma barbearia, utilizando **HTML e CSS**, seguindo os layouts desenvolvidos no Figma.

O projeto possui versões para **Desktop e Mobile**, navegação entre páginas e fluxos construídos sem JavaScript, utilizando recursos do próprio HTML e CSS, como `:target`, `:checked` e `:has()`.

---

## 🔗 Links

- **Repositório:** [Barbearia PD](https://github.com/GabrielHGB/Barbearia-PdCase)
- **Figma:** [Barbearia — Barber Club](https://www.figma.com/design/gJOVePKGs4rmqMAKgxrRNk/Barbearia-%E2%80%94-Barber-Club?node-id=1-3&t=llVgf54YF9iojENq-1)
- **Vercel:** [Barbearia PD](https://barbearia-pd-case.vercel.app/)

---

## Tecnologias utilizadas

- HTML5
- CSS3
- Figma
- Git
- GitHub

O projeto foi desenvolvido sem JavaScript.

---

## Responsividade

As interfaces foram desenvolvidas considerando principalmente os seguintes tamanhos de referência:

### Desktop

```text
Viewport: 1440px
Conteúdo máximo: 1200px
Margem lateral: 120px
Header: 80px
```

### Mobile

```text
Viewport: 402 × 874px
Conteúdo: 362px
Margem lateral: 20px
Header: 60px
```

---

## Estrutura do projeto

```text
Barbearia-PdCase
│
├── assets
│   │
│   ├── img
│   │   ├── Acabamento.png
│   │   ├── Aline.png
│   │   ├── AndréBarbeiro.png
│   │   ├── BarbaPremium.png
│   │   ├── Bruna.png
│   │   ├── ComboCompleto.png
│   │   ├── CorteClassico.png
│   │   ├── GabrielBarbeiro.png
│   │   ├── GaleriaCabelo02.png
│   │   ├── GaleriaCorte.png
│   │   ├── GaleriaCorteFreestyle.png
│   │   ├── LucasBarbeiro.png
│   │   └── PDBarber.png
│   │
│   ├── Pages
│   │   ├── Servicos.html
│   │   ├── DetalhesServicos.html
│   │   ├── Profissionais.html
│   │   ├── Galeria.html
│   │   ├── Sobre.html
│   │   ├── Planos.html
│   │   └── Agendamentos.html
│   │
│   └── Styles
│       ├── Inicio.css
│       ├── Servicos.css
│       ├── DetalhesServicos.css
│       ├── Profissionais.css
│       ├── Galeria.css
│       ├── Sobre.css
│       ├── Planos.css
│       └── Agendamentos.css
│
├── index.html
└── README.md
```

---

## Páginas do projeto

O projeto é composto pelas seguintes telas:

1. **Início**
2. **Serviços**
3. **Detalhes do Serviço**
4. **Profissionais**
5. **Galeria**
6. **Sobre a Barbearia**
7. **Planos e Mensalidades**
8. **Agendamento**
9. **Confirmar Agendamento**
10. **Agendamento Confirmado**

---

## Fluxo principal

O fluxo principal de agendamento funciona da seguinte forma:

```text
Início
  ↓
Serviços
  ↓
Detalhes do Serviço
  ↓
Profissionais
  ↓
Galeria
  ↓
Agendamento
  ↓
Confirmar Agendamento
  ↓
Agendamento Confirmado
  ↓
Início
```

---

## Navegação sem JavaScript

Algumas páginas utilizam IDs na URL para identificar o conteúdo selecionado.

Exemplo:

```text
Galeria.html#gabriel
```

Nesse caso, o profissional selecionado é identificado utilizando `:target` no CSS.

O mesmo conceito é utilizado no fluxo entre **Galeria** e **Agendamento**:

```text
Agendamentos.html#gabriel
```

Além disso, elementos como seleção de serviço, data, horário, planos e etapas de confirmação utilizam recursos como:

```css
:target
:checked
:has()
```

permitindo criar comportamentos dinâmicos sem JavaScript.

---

## Design

O projeto visual foi desenvolvido no Figma e posteriormente utilizado como referência para a implementação em HTML e CSS.

As principais definições visuais utilizadas são:

### Tipografia

```text
Títulos:
Oswald — SemiBold

Textos:
Inter — Regular
Inter — Medium
```

### Cores

```text
Fundo:
#1F1F1F

Dourado:
#C89B5B

Texto claro:
#F0F0F0

Texto secundário:
#C3C3C3

Texto escuro:
#171717

Cards:
#FFFFFF
```

---

# Documentação

A documentação do projeto está organizada separadamente na branch:

```text
Documentos
```

Essa branch contém materiais relacionados ao desenvolvimento e organização do projeto, como:

- documentação do UI Design;
- especificações das telas;
- fluxos de navegação;
- referências do Figma;
- padrões de responsividade;
- organização dos componentes;
- decisões tomadas durante o desenvolvimento.

Para acessar a branch de documentação:

```bash
git switch Documentos
```

> A branch `Documentos` é utilizada exclusivamente para manter e organizar a documentação do projeto.

---