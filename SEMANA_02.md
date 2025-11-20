# 🟡 Semana 2: Interatividade e Visual

**Nível:** Médio
**Foco:** Manipulação de Arrays (`filter`), Lógica Condicional e Formatação.

Agora que temos dados na tela, vamos tornar a aplicação útil e agradável. O usuário deve conseguir encontrar o que procura e entender rapidamente se a moeda subiu ou caiu.

## 📋 Lista de Tarefas (Checklist)

- [ ] **Barra de Busca:** Criar um `input` de texto no topo da página e um estado `busca` para guardar o que o usuário digita.
- [ ] **Filtro:** Antes de fazer o `.map()`, use o `.filter()`.
    - A lógica é: Mostrar a moeda APENAS SE o nome dela incluir o texto digitado no input.
    - Dica: Use `.toLowerCase()` em ambos para facilitar a busca.
- [ ] **Formatação de Grana:** Criar uma função ou usar `Intl.NumberFormat` para mostrar o preço bonitinho em Reais (ex: `R$ 350.200,00`).
- [ ] **Cores Condicionais:** Analisar o campo `price_change_percentage_24h`:
    - Se for **maior que 0**: Renderizar o texto em verde (classe CSS `.positive`).
    - Se for **menor que 0**: Renderizar o texto em vermelho (classe CSS `.negative`).
- [ ] **Loading:** Adicionar um texto "Carregando..." que aparece enquanto a API não responde.

## 💡 Dica de Ouro
Para o filtro funcionar bem, lembre-se: você filtra o array original, mas **não altera o estado original**.
Exemplo: `coins.filter(coin => coin.name.includes(busca)).map(...)`

**Resultado esperado na Sexta-feira:**
Um dashboard onde posso digitar "Bit" para filtrar o Bitcoin, ver o preço formatado em BRL e saber pela cor se ele valorizou ou desvalorizou hoje.