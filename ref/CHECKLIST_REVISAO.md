# CHECKLIST DE REVISAO

> **Use este documento para verificar se tudo foi implementado corretamente**
> **Versao:** 1.5 | **Data:** 2026-01-21

---

## COMO USAR

1. Copie este checklist para cada pagina que criar/revisar
2. Marque cada item conforme for verificando
3. NAO publique ate todos os itens estarem marcados

---

# CHECKLIST PAGINA DE TRILHA (INDEX)

## 1. ERROS CRITICOS (OBRIGATORIO)

- [ ] **Botoes a ESQUERDA** - Verificar `justify-start` (NAO center)
- [ ] **Numeros em circulo** - NAO esta usando setas nos topicos
- [ ] **3 secoes por topico** - Cada topico tem: O que e / Por que aprender / Conceitos-chave
- [ ] **INEMA.CLUB presente** - Link com `text-sky-400` ao lado do logo
- [ ] **Light mode CSS** - Bloco completo de overrides no `<style>`
- [ ] **Titulo modulo** - Usando `text-2xl font-bold`
- [ ] **TODOS modulos completos** - TODOS os modulos (1.1 a 1.8) devem ter topicos expandiveis, NAO apenas header+botao
- [ ] **Modal presente** - Botao "Ver em Modal" + HTML dos modais + JavaScript (openModal/closeModal)
- [ ] **Modal com iframe** - Modal deve usar `<iframe src="modulo-X-X.html">` para carregar a pagina completa (NAO conteudo duplicado)
- [ ] **2 secoes de modulos** - Primeiro cartoes simples (grid 2 cols), depois cartoes detalhados com topicos
- [ ] **Cartoes simples clicaveis** - Secao 1 usa `<a>` clicavel (SEM botoes), com hover na borda e titulo

## 2. NAVIGATION

- [ ] Logo com emoji correto do projeto
- [ ] Nome do curso visivel (hidden sm:inline em mobile)
- [ ] Separador `|` entre logo e INEMA.CLUB
- [ ] Link INEMA.CLUB com `text-sky-400 hover:text-sky-300`
- [ ] Todas as trilhas listadas com nomes completos
- [ ] Trilha atual com cor ativa (`text-[cor]-400 bg-[cor]-500/10`)
- [ ] Outras trilhas com hover correto
- [ ] Theme toggle presente com icones SVG
- [ ] Nav sticky com `backdrop-blur-sm`

## 3. HEADER

- [ ] Gradiente correto da trilha (`from-[cor]-900/30`)
- [ ] Badge "TRILHA X" com cor correta
- [ ] Titulo com emoji
- [ ] Descricao da trilha
- [ ] Stats Grid com 4 colunas:
  - [ ] Modulos
  - [ ] Topicos
  - [ ] Duracao
  - [ ] Nivel

## 4. CARDS DE MODULO

**ATENCAO:** Verificar se TODOS os 8 modulos estao completos (nao apenas alguns com topicos e outros so com header+botao)

Para cada modulo verificar:

- [ ] Numero do modulo (X.X) com cor da trilha
- [ ] Duracao (~XX min)
- [ ] Titulo com emoji e `text-2xl`
- [ ] Descricao breve
- [ ] 6-8 topicos expansiveis
- [ ] Cada topico com numero em circulo (NAO seta)
- [ ] Cada topico com emoji + titulo + subtitulo
- [ ] Conteudo expansivel com 3 secoes
- [ ] Botoes alinhados a ESQUERDA

## 5. FUNCIONALIDADE

- [ ] Toggle de topicos funcionando (abre/fecha)
- [ ] Apenas 1 topico aberto por modulo
- [ ] Theme toggle alterando dark/light
- [ ] Light mode renderizando corretamente
- [ ] Links dos botoes corretos

## 6. RESPONSIVIDADE

- [ ] Mobile: Trilhas mostram T1, T2, T3...
- [ ] Desktop: Trilhas mostram nomes completos
- [ ] Stats grid responsivo
- [ ] Cards empilham em mobile

---

# CHECKLIST PAGINA DE MODULO

## 1. ERROS CRITICOS (OBRIGATORIO)

- [ ] **Botoes navegacao** - Verificar alinhamento
- [ ] **Numeros em circulo GRANDE** - `w-12 h-12` nas secoes
- [ ] **INEMA.CLUB presente** - Link com `text-sky-400`
- [ ] **Light mode CSS** - Bloco completo de overrides no `<style>`

## 2. NAVIGATION

- [ ] Identica a pagina de trilha
- [ ] Trilha correspondente marcada como ativa

## 3. BREADCRUMB

- [ ] Presente abaixo da navigation
- [ ] Formato: Inicio / Trilha X / Modulo X.X
- [ ] Links funcionando
- [ ] Modulo atual destacado com cor da trilha

## 4. HEADER

- [ ] Gradiente correto da trilha
- [ ] Badge "MODULO X.X"
- [ ] Titulo com emoji
- [ ] Descricao do modulo
- [ ] Stats Grid com 4 colunas:
  - [ ] Topicos
  - [ ] Minutos
  - [ ] Nivel
  - [ ] Tipo

## 5. TOPICOS (SECOES)

Para cada topico (1-6) verificar:

- [ ] Numero em circulo GRANDE (`w-12 h-12`)
- [ ] Titulo h2 com emoji
- [ ] Paragrafo introdutorio
- [ ] Espacamento `mb-16` entre secoes

### Boxes de Conteudo (verificar variedade):

- [ ] Box Conceito Principal (gradiente da trilha)
- [ ] Box Dados/Pesquisa (blue)
- [ ] Box Dica Pratica (primary/yellow)
- [ ] Grid Fazer vs Evitar (emerald/red)
- [ ] Timeline (se aplicavel)
- [ ] Box Alerta (red, se aplicavel)

## 6. RESUMO FINAL

- [ ] Titulo com emoji
- [ ] Checklist do que foi aprendido (itens com ✓)
- [ ] Indicacao do proximo modulo
- [ ] Botao "Voltar para Trilha"
- [ ] Botao "Proximo Modulo"
- [ ] Gradiente correto da trilha no container

## 7. FUNCIONALIDADE

- [ ] Theme toggle funcionando
- [ ] Light mode renderizando corretamente
- [ ] Links de navegacao corretos
- [ ] IDs dos topicos para ancora (#topico-1, #topico-2, etc)

---

# CHECKLIST CORES POR TRILHA

Verificar se a trilha usa as cores corretas conforme o numero:

## Trilha 1 (Emerald)

- [ ] `text-emerald-400`
- [ ] `bg-emerald-500/20`
- [ ] `border-emerald-500/30`
- [ ] `from-emerald-900/30`

## Trilha 2 (Blue)

- [ ] `text-blue-400`
- [ ] `bg-blue-500/20`
- [ ] `border-blue-500/30`
- [ ] `from-blue-900/30`

## Trilha 3 (Purple)

- [ ] `text-purple-400`
- [ ] `bg-purple-500/20`
- [ ] `border-purple-500/30`
- [ ] `from-purple-900/30`

## Trilha 4 (Amber)

- [ ] `text-amber-400`
- [ ] `bg-amber-500/20`
- [ ] `border-amber-500/30`
- [ ] `from-amber-900/30`

## Trilha 5 (Teal)

- [ ] `text-teal-400`
- [ ] `bg-teal-500/20`
- [ ] `border-teal-500/30`
- [ ] `from-teal-900/30`

## Trilha 6 (Rose)

- [ ] `text-rose-400`
- [ ] `bg-rose-500/20`
- [ ] `border-rose-500/30`
- [ ] `from-rose-900/30`

---

# CHECKLIST JAVASCRIPT

- [ ] Funcao `toggleTopic()` presente
- [ ] Funcao fecha outros topicos do mesmo modulo
- [ ] Theme toggle inicializa icone correto
- [ ] Theme toggle salva preferencia no localStorage
- [ ] Theme toggle alterna classe `dark` no html
- [ ] Funcao `openModal()` presente (pagina de trilha)
- [ ] Funcao `closeModal()` presente (pagina de trilha)
- [ ] Modal fecha com tecla ESC

---

# CHECKLIST CSS

- [ ] Font Inter importada
- [ ] `body { font-family: 'Inter', sans-serif; }`
- [ ] `.topic-explanation { display: none; }`
- [ ] `.topic-explanation.active { display: block; }`
- [ ] Bloco completo de Light mode overrides

---

# CHECKLIST PAGINA DE SLIDES

## Estrutura
- [ ] Pasta `/curso/trilhaX/slides/` criada
- [ ] Arquivo `slides-X-X.html` para cada modulo com imagens
- [ ] Imagens referenciadas de `/doc/XX/` (pasta corresponde ao modulo)

## Layout
- [ ] Header com badge "SLIDES DO MODULO X.X"
- [ ] Stats: quantidade de slides, tempo estimado, tipo "Visual"
- [ ] Cards de slide com numero em circulo + titulo
- [ ] Imagem clicavel para zoom (modal)
- [ ] Navegacao entre slides e voltar ao modulo

## Conteudo
- [ ] **TEXTO COMPLETO E DETALHADO** - Cada slide deve ter descricao rica explicando o conteudo visual
- [ ] Contextualizacao do que esta sendo mostrado
- [ ] Conceitos-chave destacados em negrito
- [ ] Conexao com o conteudo do modulo

## Funcionalidade
- [ ] Modal de zoom funcionando (clique na imagem)
- [ ] Fechar modal com ESC
- [ ] Theme toggle funcionando
- [ ] Light mode renderizando

## Botoes (onde adicionar)
- [ ] Botao roxo "📊 Ver Slides" na pagina do modulo (ao lado de navegacao)
- [ ] Botao roxo "📊 Slides" no card detalhado do index da trilha

## Mapeamento de Pastas
| Pasta doc | Modulo |
|-----------|--------|
| doc/11 | 1.1 |
| doc/12 | 1.2 |
| doc/13 | 1.3 |

---

# VERIFICACAO FINAL

Antes de publicar, responda:

1. [ ] Abri a pagina no navegador?
2. [ ] Testei o dark mode?
3. [ ] Testei o light mode?
4. [ ] Cliquei em todos os topicos expansiveis?
5. [ ] Verifiquei todos os links?
6. [ ] Testei em mobile (ou redimensionei a janela)?
7. [ ] Comparei visualmente com uma pagina existente que esta correta?

---

# TEMPLATE RAPIDO PARA COPIAR

```
## Revisao: [Nome da Pagina]
Data: ____/____/____

### Erros Criticos
- [ ] Botoes ESQUERDA
- [ ] Numeros em circulo
- [ ] 3 secoes por topico
- [ ] INEMA.CLUB
- [ ] Light mode CSS
- [ ] Titulo text-2xl
- [ ] Modulos completos (index)
- [ ] Modal funcionando (index)
- [ ] Cartoes simples clicaveis (index)

### Estrutura
- [ ] Navigation completa
- [ ] Header com stats
- [ ] Conteudo correto
- [ ] Resumo/navegacao

### Funcional
- [ ] Dark mode OK
- [ ] Light mode OK
- [ ] Links OK
- [ ] Responsivo OK

### Status: [ ] APROVADO / [ ] PENDENTE
```

---

# ERROS MAIS COMUNS (REVISAR ESPECIALMENTE)

| Erro | O que verificar |
|------|-----------------|
| Botoes centralizados | Procurar por `justify-center` nos botoes de modulo |
| Setas em vez de numeros | Procurar por `▶` ou `→` nos topicos |
| Faltando INEMA.CLUB | Verificar navigation |
| Light mode quebrado | Testar alternando o tema |
| Titulo pequeno | Verificar se h3 do modulo tem `text-2xl` |
| Cor errada | Comparar com tabela de cores da trilha |
| Topico sem 3 secoes | Abrir cada topico e verificar |
| Modulos incompletos no index | Verificar se TODOS os modulos tem topicos expandiveis (nao apenas header+botao) |
| Modal faltando | Verificar botao "Ver em Modal", HTML dos modais e funcoes openModal/closeModal |
| Modal sem iframe | Modal DEVE usar `<iframe src="modulo-X-X.html">` para carregar pagina completa |
| Faltando secao de cartoes simples | Index deve ter: 1) Cartoes simples (grid 2 cols) 2) Cartoes detalhados com topicos |
| Cartoes simples com botoes | Secao 1 deve usar `<a>` clicavel, SEM botoes - apenas hover na borda/titulo |

---

**Ultima atualizacao:** 2026-01-21
**Versao:** 1.5
