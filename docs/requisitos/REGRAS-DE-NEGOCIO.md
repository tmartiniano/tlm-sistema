# Regras de negócio

## Custos

A base de cálculo é sempre o valor bruto da venda.

### Comissão

Comissão de 20% sobre toda venda:

- Dinheiro: sim
- Cartão de crédito: sim
- Cartão de débito: sim
- Pix: sim

### Taxa de pagamento

Taxa de 2% sobre o valor bruto:

- Dinheiro: não
- Cartão de crédito: sim
- Cartão de débito: sim
- Pix: sim

## Fórmulas

```text
comissao = valor_bruto * 0,20

taxa_pagamento =
  dinheiro: 0
  cartão ou Pix: valor_bruto * 0,02

custos_operacionais = comissao + taxa_pagamento

resultado_estimado =
  valor_bruto - custos_operacionais
```

## Descontos

Descontos não reduzem a base de cálculo dos custos.

## Cancelamentos e estornos

Pedidos cancelados ou estornados não geram comissão nem taxa.
