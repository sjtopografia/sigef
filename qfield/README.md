# SJ GeoField — Projetos QField por UF

Coleção de projetos prontos para **QGIS** e **QField**, organizados por unidade da federação e modalidade de acesso aos dados.

A estrutura prevê **54 projetos independentes**:

- 27 projetos **WMS**, um para cada UF;
- 27 projetos **WFS**, um para cada UF.

WMS e WFS são distribuídos em arquivos `.qgz` separados.

## Estrutura prevista

```text
qfield/
├── README.md
├── docs/
│   ├── instalacao-qfield.md
│   ├── estrutura-dos-projetos.md
│   ├── fontes-de-dados.md
│   ├── wms-vs-wfs.md
│   ├── limitacoes-wfs.md
│   ├── simbologia-wfs.md
│   └── licencas-e-creditos.md
└── projetos/
    ├── WMS/
    │   ├── AC/
    │   ├── AL/
    │   ├── ...
    │   └── TO/
    └── WFS/
        ├── AC/
        ├── AL/
        ├── ...
        └── TO/
```

## Projeto WMS

Indicado principalmente para **visualização e navegação em campo**.

Características:

- serviços WMS do INCRA;
- OpenStreetMap como mapa-base;
- menor carga no dispositivo em comparação com WFS;
- atributos disponíveis somente quando o serviço suportar `GetFeatureInfo`;
- cores e estilos principais dependem da renderização do servidor WMS.

## Projeto WFS

Indicado quando o usuário precisa de **geometria vetorial e atributos**.

Características:

- serviços WFS do INCRA;
- OpenStreetMap como mapa-base;
- geometrias vetoriais;
- atributos completos conforme disponibilizados pelo serviço;
- maior consumo de memória, processamento e dados em dispositivos móveis;
- camadas devem permanecer desligadas por padrão e ser ativadas apenas quando necessárias.

## Simbologia categorizada no WFS

A simbologia dos imóveis é categorizada pelo atributo `status`.

- `CERTIFICADA` → azul-claro, preenchimento com 50% de transparência;
- `REGISTRADA` → roxo-escuro, preenchimento com 50% de transparência;
- demais valores → purple, preenchimento com 50% de transparência;
- limites → linha branca contínua mais grossa com linha preta pontilhada sobreposta.

A categorização é aplicada pelo cliente QGIS/QField. Ela não é aplicada ao WMS, cuja imagem já vem renderizada pelo servidor.

## OpenStreetMap

O OpenStreetMap é utilizado como mapa-base nos projetos.

Atribuição:

`© OpenStreetMap contributors`

## Desenvolvimento e configuração

**SJ Topografia**  
Instagram: [@sj.topografia](https://www.instagram.com/sj.topografia/)

## Independência

Este projeto é independente e não é afiliado, patrocinado ou endossado pelo QGIS, QField, INCRA ou OpenStreetMap Foundation.
