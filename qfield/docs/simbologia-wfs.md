# Simbologia WFS

A simbologia dos imóveis é categorizada pelo atributo `status`.

## Categorias

| Valor de `status` | Preenchimento | Transparência |
|---|---|---:|
| `CERTIFICADA` | azul-claro | 50% |
| `REGISTRADA` | roxo-escuro | 50% |
| demais valores | purple | 50% |

A expressão de categorização deve normalizar espaços e caixa para que valores equivalentes sejam tratados corretamente.

Exemplo conceitual:

```text
upper(trim(coalesce("status", '')))
```

## Limites

As bordas dos polígonos utilizam duas linhas sobrepostas:

1. linha branca contínua, mais grossa;
2. linha preta pontilhada, mais fina.

Essa composição melhora o contraste sobre mapas-base claros e escuros.

## WMS

Essa categorização não é aplicada ao projeto WMS, porque o WMS entrega uma imagem já renderizada pelo servidor. No WMS, as cores e bordas dependem do estilo publicado no serviço.
