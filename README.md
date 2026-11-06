# STUCK - Gestão de encomendas

Ferramenta web leve para importar relatórios em CSV e revisar pedidos por status, estação atual e tempo desde a recepção.

## O que faz
- Importa um CSV com o cabeçalho da planilha usada na operação.
- Exibe apenas os campos essenciais: Order ID, rastreio, status, estação atual e data de recebimento.
- Calcula a idade do pedido a partir do campo `Received Time` e destaca pedidos em situação crítica quando o status é `Hub_Received` ou `Hub_Assigned`.
- Permite busca por pedido, rastreio ou estação e filtro por status.
- Exporta um CSV reduzido com os campos essenciais.

## Como usar
1. Abra o arquivo `index.html` no navegador.
2. Importe o CSV da operação.
3. Use a busca e os filtros por status para focar os pedidos relevantes.
4. Verifique os pedidos em destaque e exporte quando necessário.

## Observações
- Os dias mostrados são calculados a partir do campo `Received Time` e da data atual do navegador.
- Os dados ficam apenas na memória da página enquanto a aba estiver aberta; não há armazenamento persistente nesta versão.
