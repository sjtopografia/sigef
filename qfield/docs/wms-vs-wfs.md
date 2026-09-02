# WMS x WFS

No SJ GeoField, WMS e WFS são distribuídos em projetos separados.

## WMS

Entrega imagens renderizadas pelo servidor.

Uso recomendado:
- navegação;
- visualização;
- uso em campo;
- dispositivos móveis.

Características:
- menor processamento local;
- sem geometria vetorial no cliente;
- atributos dependem de `GetFeatureInfo`;
- estilo principal vem do servidor.

## WFS

Entrega feições vetoriais e atributos.

Uso recomendado:
- consulta de atributos;
- seleção de feições;
- acesso à geometria;
- análises vetoriais.

Características:
- maior volume de dados;
- maior consumo de memória;
- risco de timeout em grandes áreas;
- maior sensibilidade em dispositivos móveis.

## Escolha prática

Para enxergar e navegar: **WMS**.

Para geometria e atributos: **WFS**.
