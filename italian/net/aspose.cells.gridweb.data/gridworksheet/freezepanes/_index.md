---
title: "GridWorksheet.FreezePanes"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "GridWorksheet metodo. Congela i riquadri nella cella specificata del foglio di lavoro"
type: docs
url: /it/net/aspose.cells.gridweb.data/gridworksheet/freezepanes/
---
## FreezePanes(string, int, int) {#freezepanes_1}

Blocca i riquadri nella cella specificata nel foglio di lavoro.

```csharp
public void FreezePanes(string cellName, int freezedRows, int freezedColumns)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cellName | String | Nome della cella. |
| freezedRows | Int32 | Numero di righe visibili nel riquadro superiore, non più dell'indice di riga. |
| freezedColumns | Int32 | Numero di colonne visibili nel riquadro sinistro, non più dell'indice di colonna. |

### Osservazioni

L'indice di riga e l'indice di colonna non possono entrambi essere zero. Anche il numero di righe e il numero di colonne non possono entrambi essere zero.

### Vedi anche

* class [GridWorksheet](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## FreezePanes(int, int, int, int) {#freezepanes}

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

* class [GridWorksheet](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


