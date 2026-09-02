# Limitações do WFS em dispositivos móveis

O projeto WFS é separado do WMS para que o usuário escolha quando precisa carregar dados vetoriais.

Em grandes extensões podem ocorrer:

- lentidão;
- timeout;
- alto consumo de memória;
- alto consumo de dados móveis;
- demora na renderização;
- carregamento parcial.

## Recomendações

- mantenha as camadas WFS desligadas por padrão;
- ative apenas as camadas necessárias;
- trabalhe em escalas locais;
- evite ativar simultaneamente várias camadas estaduais;
- use o projeto WMS para navegação comum.
