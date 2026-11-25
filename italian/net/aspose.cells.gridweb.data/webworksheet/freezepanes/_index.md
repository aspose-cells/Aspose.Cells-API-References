---
title: "WebWorksheet.FreezePanes"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo WebWorksheet. Congela i riquadri nella cella specificata del foglio di lavoro"
type: docs
url: /it/net/aspose.cells.gridweb.data/webworksheet/freezepanes/
---
## WebWorksheet.FreezePanes method

Blocca i riquadri nella cella specificata nel foglio di lavoro.

```csharp
public void FreezePanes(int row, int column, int freezedRows, int freezedColumns)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | Int32 | Indice della riga. |
| colonna | Int32 | Indice colonna. |
| freezedRows | Int32 | Numero di righe visibili nel riquadro superiore, non più dell'indice di riga. |
| freezedColumns | Int32 | Numero di colonne visibili nel riquadro sinistro, non più dell'indice di colonna. |

### Osservazioni

L'indice di riga e l'indice di colonna non possono entrambi essere zero. Anche il numero di righe e il numero di colonne non possono entrambi essere zero.

I primi due parametri specificano la posizione congelata e gli ultimi due parametri specificano l'area congelata sul riquadro in alto a sinistra.

### Vedi anche

* class [WebWorksheet](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


