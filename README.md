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

## 🎓 **Nota Avaliativa**

### **5.5 / 10.0** + Ponto_Extra 5 = 10.0

| Critério | Nota | Justificativa |
|----------|------|--------------|
| **Semântica HTML5** | 6.0 | Uso correto das tags principais, mas estrutura de tabela incorreta |
| **Estrutura de Formulário** | 4.5 | Labels sem `for/id`, inputs sem `name`, faltam validações |
| **Limpeza de Código** | 7.5 | Sem div soup, mas com indentação inconsistente |
| **Acessibilidade** | 4.0 | Faltam atributos essenciais (name, id, required) |
| **Ponto Extra** | +5.0 | Esforço do grupo e estrutura básica bem definida |

---

### **Recomendações Prioritárias:**
1. ⚠️ Corrigir a estrutura da tabela imediatamente
2. ⚠️ Adicionar `id`, `name` e `for` aos formulários
3. ⚠️ Incluir validações (`required`, `placeholder`)
4. ⚠️ Adicionar `<nav>` para navegação semântica
