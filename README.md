# Projeto Grupo 4

Jane \ Raiane \ Kellyane

---

## 📋 Avaliação do Código HTML

### ✅ **Pontos Positivos**

1. **Estrutura Semântica Base**: Uso correto de `<header>`, `<main>` e `<footer>`
2. **Tipos de Input Apropriados**: Uso de `<input type="date">` e `<input type="time">` 
3. **Sem Div Soup**: Não há uso excessivo de `<div>` desnecessários
4. **Meta Tags Essenciais**: Charset UTF-8 e viewport presentes

---

### ❌ **Problemas Críticos**

#### 1. **Estrutura de Tabela Incorreta** (Erro Grave)
- `<thead>` contendo `<tbody>` (inversão de ordem)
- `<th>` envolvendo `<td>` (semanticamente incorreto)
- Falta de dados reais na tabela

#### 2. **Formulário sem Semântica Apropriada**
- `label for=""` vazio (desassociado)
- `input name=""` e `id=""` vazios
- `<select>` sem `name` e sem `label` associada
- Falta `required` nos campos obrigatórios

#### 3. **Falta de Navegação Semântica**
- Ausência de `<nav>` para navegação
- Sem seções adequadamente estruturadas

#### 4. **Acessibilidade Deficiente**
- Faltam atributos essenciais para associação de elementos
- Sem validações de formulário (`required`, `placeholder`)

---

## 🎓 **Nota Avaliativa - HTML**

### **5.5 / 10.0** + Ponto_Extra 5 = 10.0

| Critério | Nota | Justificativa |
|----------|------|--------------|
| **Semântica HTML5** | 6.0 | Uso correto das tags principais, mas estrutura de tabela incorreta |
| **Estrutura de Formulário** | 4.5 | Labels sem `for/id`, inputs sem `name`, faltam validações |
| **Limpeza de Código** | 7.5 | Sem div soup, mas com indentação inconsistente |
| **Acessibilidade** | 4.0 | Faltam atributos essenciais (name, id, required) |
| **Ponto Extra** | +5.0 | Esforço do grupo e estrutura básica bem definida |

---

### **Recomendações Prioritárias (HTML):**
1. ⚠️ Corrigir a estrutura da tabela imediatamente
2. ⚠️ Adicionar `id`, `name` e `for` aos formulários
3. ⚠️ Incluir validações (`required`, `placeholder`)
4. ⚠️ Adicionar `<nav>` para navegação semântica

---

## 🎨 Avaliação do Código CSS

### 📊 Resumo Geral
O código demonstra **conhecimento básico de Flexbox e Media Queries**, mas apresenta **problemas estruturais significativos** e **falta de organização** que prejudicam a manutenibilidade e qualidade.

---

### ✅ Pontos Positivos

| Critério | Avaliação |
|----------|-----------|
| **Flexbox** | Uso correto em `main` com `flex-direction: column`, `justify-content` e `align-items` |
| **Media Queries** | Presente e estruturado para mobile (768px) |
| **Reset CSS** | Bom início com `* { margin:0; padding:0; box-sizing: border-box; }` |
| **Botões** | Hover effect implementado corretamente |

---

### ❌ Problemas Críticos

#### 1. **Erros de Propriedades CSS** 🔴
```css
/* ❌ ERRADO - border não aceita apenas número */
border-bottom: 20px;     /* Deveria ser: border-bottom: 2px solid #ccc; */
border: 20px;            /* Deveria ser: border: 2px solid #ccc; */

/* ❌ ERRADO - box-shadow não funciona assim */
box-shadow: 40px;        /* Deveria ser: box-shadow: 0 4px 8px rgba(0,0,0,0.2); */
```

#### 2. **Falta de Organização** 🔴
- Sem divisão por seções (reset, layout, componentes, etc.)
- Sem variáveis CSS para cores (está repetindo `rgb(93, 201, 225)` em vários lugares)
- Sem comentários explicativos

#### 3. **Hierarquia Visual Fraca** 🔴
```css
/* Não há distinção clara entre diferentes níveis de importância */
header { padding: 50px; }    /* Grande demais? */
footer { padding: 20px; }    /* Pequeno demais? */
button { font-size: 20px; }  /* Sem peso visual diferenciado */
```

#### 4. **Responsividade Incompleta** 🟡
- Media query está com sintaxe errada: `@media screen and (max-width:768px)` deveria ser `@media screen and (max-width: 768px)`
- Faltam breakpoints para tablets e desktop
- `input` e `select` não têm ajustes responsivos

---

### 📋 Checklist de Melhoria

- [ ] Usar **variáveis CSS** (`:root`) para cores e espaçamento
- [ ] **Organizar** o arquivo em seções comentadas
- [ ] **Corrigir** erros de propriedades (`border`, `box-shadow`)
- [ ] Adicionar **múltiplos breakpoints** (mobile, tablet, desktop)
- [ ] Criar **hierarquia visual** clara (tamanhos de fonte, pesos, cores)
- [ ] Implementar **transições** para melhor UX
- [ ] Adicionar **documentação** através de comentários

---

## 🎓 **Nota Avaliativa - CSS**

### **4.5 / 10.0**

| Critério | Nota | Justificativa |
|----------|------|--------------|
| **Flexbox/Grid** | 6.5 | Uso correto de Flexbox em `main`, mas limitado em outras áreas |
| **Media Queries** | 5.0 | Presente mas com erros de sintaxe e breakpoints insuficientes |
| **Organização** | 3.0 | Sem variáveis CSS, sem comentários, sem estrutura de seções |
| **Hierarquia Visual** | 3.5 | Não há distinção clara entre elementos principais e secundários |
| **Propriedades CSS** | 2.5 | Erros graves em `border`, `box-shadow` (valores inválidos) |

---

### **Recomendações Prioritárias (CSS):**
1. ⚠️ **URGENTE**: Corrigir propriedades CSS inválidas (`border: 20px`, `box-shadow: 40px`)
2. ⚠️ Implementar variáveis CSS para cores e espaçamento
3. ⚠️ Organizar o arquivo em seções comentadas
4. ⚠️ Adicionar breakpoints para tablet e desktop
5. ⚠️ Melhorar hierarquia visual com tamanhos e pesos de fonte diferenciados

---

## 📈 Resumo Geral do Projeto

| Componente | Nota | Status |
|-----------|------|--------|
| **HTML** | 10.0/10 | ✅ Bom (com ponto extra) |
| **CSS** | 4.5/10 | ⚠️ Precisa melhorias estruturais |
| **JavaScript** | — | — |
| **Média Atual** | **7.25/10** | — |

**Próximos passos**: Focar em corrigir os erros CSS e melhorar a organização do código antes de adicionar funcionalidades JavaScript.
