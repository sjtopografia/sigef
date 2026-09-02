# Estrutura dos projetos

O SJ GeoField distribui WMS e WFS em projetos separados.

## WMS por UF

```text
SJ GeoField — WMS — UF
│
├── 10 - INCRA WMS
│   ├── 01 - SIGEF
│   ├── 02 - Certificação anterior / SNCI
│   ├── 03 - Parcelas
│   ├── 04 - Reforma Agrária
│   └── 05 - Territórios
│
└── 99 - Mapa base
    └── OpenStreetMap
```

## WFS por UF

```text
SJ GeoField — WFS — UF
│
├── 20 - INCRA WFS
│   ├── 01 - SIGEF
│   ├── 02 - Certificação anterior / SNCI
│   ├── 03 - Parcelas
│   ├── 04 - Reforma Agrária
│   └── 05 - Territórios
│
└── 99 - Mapa base
    └── OpenStreetMap
```

## Quantidade

27 UFs × 2 modalidades = **54 projetos**.
