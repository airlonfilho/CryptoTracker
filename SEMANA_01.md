# 🟢 Semana 1: O Início

**Nível:** Fácil
**Foco:** Consumo de API (`useEffect`), Estados (`useState`) e Listas (`map`).

Nesta primeira semana, o objetivo é simples: **Fazer os dados aparecerem na tela.** Não se preocupe com filtros ou navegação agora. Foque em garantir que a conexão com a API funciona e que o React consegue renderizar a lista.

## 📋 Lista de Tarefas (Checklist)

- [ ] **Limpeza:** Apagar os arquivos padrões do Vite (App.css, logos desnecessários) e deixar o `App.jsx` limpo.
- [ ] **Estado:** Criar um `useState([])` para armazenar a lista de moedas (inicialize como array vazio).
- [ ] **Requisição:** Criar um `useEffect` que executa apenas uma vez ao montar a página.
    - Dentro dele, fazer o `fetch` para a URL da API da CoinGecko.
    - Converter a resposta para JSON.
    - Salvar os dados no seu estado (setCoins).
- [ ] **Renderização:** Usar o método `.map()` no seu estado para exibir as moedas na tela.
- [ ] **Interface:** Cada item da lista deve mostrar pelo menos:
    - Nome da moeda.
    - Símbolo (ex: btc).
    - Preço atual (pode ser sem formatação por enquanto).

## 💡 Dica de Ouro
Se a tela ficar branca ou der erro, abra o **Console do Navegador** (F12). Verifique se o array de dados está chegando corretamente com um `console.log(dados)` antes de salvar no estado.

**Resultado esperado na Sexta-feira:**
Uma página que, ao ser recarregada, mostra uma lista simples (pode ser feia) com as 10 principais moedas e seus preços.