# 🔴 Semana 3: Roteamento e Detalhes

**Nível:** Difícil
**Foco:** React Router DOM, Rotas Dinâmicas e SPA (Single Page Application).

Esta é a etapa que transforma seu "exercício" em um "projeto profissional". Vamos criar uma segunda página para ver os detalhes profundos de uma moeda específica.

## 📋 Lista de Tarefas (Checklist)

- [ ] **Instalação:** Instalar a biblioteca de rotas: `npm install react-router-dom`.
- [ ] **Configuração:** Configurar o `BrowserRouter`, `Routes` e `Route` no seu `main.jsx` ou `App.jsx`.
- [ ] **Nova Tela:** Criar um componente/página novo chamado `CoinDetails.jsx`.
- [ ] **Linkagem:** Na lista da Home (semana 1 e 2), transformar o nome da moeda em um `<Link>` que leva para `/coin/ID_DA_MOEDA`.
- [ ] **Rota Dinâmica:** Configurar a rota para aceitar parâmetros (ex: `/coin/:id`).
- [ ] **Hook de Parâmetros:** Na página `CoinDetails`, usar o hook `useParams()` para descobrir qual moeda foi clicada.
- [ ] **Nova Requisição:** Na página de detalhes, fazer um novo `useEffect` que busca dados específicos daquela moeda.
    - Endpoint: `https://api.coingecko.com/api/v3/coins/{id}`
- [ ] **Exibir Detalhes:** Mostrar a descrição da moeda (campo `description.en`), imagem grande e data de criação.
- [ ] **Botão Voltar:** Criar um botão/link para retornar à Home.

## 💡 Dica de Ouro
O endpoint de detalhes retorna um objeto MUITO grande e complexo. Use `console.log` para investigar onde está a descrição da moeda dentro desse objeto (geralmente está aninhada).

**Resultado esperado na Sexta-feira:**
Um site completo. Clico no Bitcoin na Home, sou levado para uma página só dele com texto explicativo e logo grande, e posso clicar em "Voltar" para pesquisar outra moeda.