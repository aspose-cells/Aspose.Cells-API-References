---
title: "Worksheet.FreezePanes"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Worksheet. Congela i riquadri nella cella specificata del foglio di lavoro"
type: docs
url: /it/net/aspose.cells/worksheet/freezepanes/
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

I primi due parametri specificano la posizione di congelamento e gli ultimi due parametri specificano l'area congelata nel riquadro superiore sinistro.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodFreezePanesWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Congela i riquadri alla riga 3, colonna 3, con 3 righe congelate e 3 colonne congelate
            worksheet.FreezePanes(3, 3, 3, 3);
            
            // Salva la cartella di lavoro
            workbook.Save("FreezePanesDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

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

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodFreezePanesWithStringInt32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Congela i riquadri a "C3" con 3 righe congelate e 3 colonne congelate
            worksheet.FreezePanes("C3", 3, 3);

            // Salva la cartella di lavoro
            workbook.Save("FreezePanesDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


