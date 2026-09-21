# 03 - UI Design — PD Barber

Esta seção contém as telas finais da interface da **PD Barber**, desenvolvidas a partir dos wireframes e posteriormente utilizadas como referência para a implementação em HTML e CSS.

O UI Design deve manter consistência entre **Desktop** e **Mobile**, utilizando os mesmos componentes, estilos, tipografia, cores, espaçamentos e padrões visuais definidos no projeto.

---

## 📱 Tamanhos de referência

### Desktop

- Frame: `1440px`
- Conteúdo máximo: `1200px`
- Margem lateral de segurança: `120px`
- Header: `80px`

### Mobile

- Frame: `402 × 874px`
- Conteúdo: `362px`
- Margem lateral: `20px`
- Header: `60px`

---

# 🎨 Design System

## Tipografia

### Títulos

- Fonte: `Oswald`
- Peso: `SemiBold`

Utilizada em:

- títulos de páginas;
- títulos de seções;
- nomes de serviços;
- nomes de profissionais;
- preços em destaque;
- títulos de cards.

### Textos

- Fonte: `Inter`
- Pesos:
  - `Regular`
  - `Medium`

Utilizada em:

- descrições;
- informações auxiliares;
- botões;
- navegação;
- textos dos cards.

---

## Cores principais

```text
Fundo principal:
#1F1F1F

Dourado:
#C89B5B

Texto claro:
#F0F0F0

Texto secundário:
#C3C3C3

Texto escuro:
#171717

Cards claros:
#FFFFFF
```

---

# 🖥️ Telas

## 01 - Início

Tela principal da barbearia.

### Conteúdo

- Header
- Hero
  - título principal;
  - descrição;
  - CTA `AGENDAR HORÁRIO`;
  - imagem principal.
- Serviços em destaque
- Profissionais em destaque
- Chamada para planos

### Fluxos

```text
AGENDAR HORÁRIO
→ Profissionais

Serviço
→ Detalhes do Serviço

Profissional
→ Galeria

VER PLANOS
→ Planos e Mensalidades
```

---

## 02 - Serviços

Apresenta os serviços disponíveis na barbearia.

### Conteúdo

- Título da página
- Introdução
- Campo de busca
- Filtros
  - Todos
  - Corte
  - Barba
- Lista de serviços

### Serviços

- Corte Clássico
- Barba Premium
- Combo Completo
- Acabamento

### Fluxo

```text
Serviço selecionado
→ Detalhes do Serviço
```

---

## 03 - Detalhes do Serviço

Apresenta informações detalhadas sobre um serviço.

### Conteúdo

- Imagem principal
- Nome do serviço
- Preço
- Descrição
- Profissionais disponíveis
- Galeria de trabalhos
- CTA para escolher profissional

### Fluxo

```text
ESCOLHER PROFISSIONAL
→ Profissionais
```

---

## 04 - Profissionais

Permite selecionar o profissional desejado.

### Profissionais

- Gabriel
- Lucas
- André
- Bruna
- Aline

### Conteúdo do card

- Foto
- Nome
- Especialidade
- CTA de seleção

### Fluxo

```text
SELECIONAR
→ Galeria do profissional
```

Exemplo:

```text
Galeria.html#gabriel
```

---

## 05 - Galeria

Exibe informações e trabalhos recentes do profissional selecionado.

### Conteúdo

- Informações do profissional
  - foto;
  - nome;
  - especialidade.
- Trabalhos recentes
  - imagem principal;
  - duas imagens secundárias.
- CTA de agendamento

### Fluxo

```text
AGENDAR COM PROFISSIONAL
→ Agendamento
```

Exemplo:

```text
Agendamentos.html#gabriel
```

---

## 06 - Sobre a Barbearia

Apresenta informações institucionais da PD Barber.

### Conteúdo

- Imagem da barbearia
- Sobre a barbearia
- Texto institucional
- Indicadores
  - `+5` anos de experiência
  - `+1K` atendimentos
- Contato
  - WhatsApp
  - Instagram
- Horário de funcionamento

---

## 07 - Planos e Mensalidades

Apresenta os planos disponíveis.

### Essencial

```text
R$ 79/mês
```

- 2 cortes por mês
- Prioridade no agendamento

### Signature

```text
R$ 129/mês
```

- 2 cortes
- 2 barbas
- Prioridade no agendamento

O plano `Signature` possui destaque visual.

### Black

```text
R$ 179/mês
```

- 4 serviços por mês
- Prioridade máxima

### Estados

Os cards devem possuir:

```text
Default
Hover
Selecionado
```

---

## 08 - Agendamento

Tela utilizada para selecionar as informações do atendimento.

### Conteúdo

#### Serviço

- Corte Clássico
- Barba Premium
- Combo Completo
- Acabamento

#### Dia

Lista de datas disponíveis.

#### Horário

Lista de horários disponíveis.

#### Comentários

Campo opcional para observações.

### Fluxo

```text
AGENDAR
→ Confirmar Agendamento
```

---

## 09 - Confirmar Agendamento

Tela utilizada para revisar as informações antes da confirmação.

### Conteúdo

#### Profissional

Profissional selecionado anteriormente.

#### Serviço

Serviço selecionado + valor.

#### Dia do agendamento

Data escolhida.

#### Horário

Horário escolhido.

### Ações

```text
CONFIRMAR AGENDAMENTO
→ Agendamento Confirmado
```

```text
ALTERAR DATA OU HORÁRIO
→ Agendamento
```

---

## 10 - Agendamento Confirmado

Tela final do fluxo de agendamento.

### Conteúdo

- Ícone de confirmação
- Título: `AGENDAMENTO CONFIRMADO!`
- Mensagem: `Seu horário foi reservado com sucesso.`
- Texto complementar: `Esperamos você na PD Barber.`
- CTA: `VOLTAR AO INÍCIO`

### Fluxo

```text
VOLTAR AO INÍCIO
→ Home
```

---

# 🔄 Fluxo principal

```text
HOME
  ↓
PROFISSIONAIS
  ↓
GALERIA
  ↓
AGENDAMENTO
  ↓
CONFIRMAR AGENDAMENTO
  ↓
AGENDAMENTO CONFIRMADO
  ↓
HOME
```

Fluxo de serviços:

```text
SERVIÇOS
  ↓
DETALHES DO SERVIÇO
  ↓
PROFISSIONAIS
```

---

# 📂 Organização no Figma

```text
03 - UI Design
│
├── 01 - Início
│   ├── Desktop
│   └── Mobile
│
├── 02 - Serviços
│   ├── Desktop
│   └── Mobile
│
├── 03 - Detalhes do Serviço
│   ├── Desktop
│   └── Mobile
│
├── 04 - Profissionais
│   ├── Desktop
│   └── Mobile
│
├── 05 - Galeria
│   ├── Desktop
│   └── Mobile
│
├── 06 - Sobre a Barbearia
│   ├── Desktop
│   └── Mobile
│
├── 07 - Planos e Mensalidades
│   ├── Desktop
│   └── Mobile
│
├── 08 - Agendamento
│   ├── Desktop
│   └── Mobile
│
├── 09 - Confirmar Agendamento
│   ├── Desktop
│   └── Mobile
│
└── 10 - Agendamento Confirmado
    ├── Desktop
    └── Mobile
```

---

# 🧩 Componentes compartilhados

Sempre que possível, reutilizar componentes para:

- Header
- Botão
- Título de seção
- Card de serviço
- Card de profissional
- Card de plano
- Opção de seleção
- Campo de formulário
- Imagem de galeria
- CTA

A reutilização dos componentes garante consistência visual e facilita alterações globais no projeto.

---

# 📏 Padrões de espaçamento

## Mobile

```text
Viewport: 402px
Conteúdo: 362px
Margem lateral: 20px
Header: 60px
```

## Desktop

```text
Viewport: 1440px
Conteúdo máximo: 1200px
Margem lateral: 120px
Header: 80px
```

Os espaçamentos internos devem seguir uma escala consistente, priorizando valores como:

```text
4px
8px
10px
12px
16px
18px
20px
24px
32px
40px
48px
```

---

# ✅ Diretrizes finais

- Todas as telas devem possuir versão `Desktop` e `Mobile`.
- O UI Design deve representar o comportamento implementado no código.
- Os elementos devem utilizar Auto Layout sempre que possível.
- Os componentes devem ser reutilizados entre telas.
- O fluxo de navegação deve estar atualizado com a implementação real.
- A seleção de profissional segue o fluxo `Profissionais → Galeria → Agendamento`.
- O fluxo de agendamento segue `Agendamento → Confirmar Agendamento → Agendamento Confirmado`.
- A tela `10 - Agendamento Confirmado` deve existir em Desktop e Mobile.
- A estrutura visual deve manter as mesmas proporções utilizadas na implementação HTML/CSS.