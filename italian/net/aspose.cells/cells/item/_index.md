---
title: "Cells.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cells. Ottiene l'elemento Cell all'indice di riga e colonna specificati"
type: docs
url: /it/net/aspose.cells/cells/item/
---
## Cells indexer (1 of 2)

Ottiene l'elemento [`Cell`](../../cell/) all'indice di riga e colonna della cella specificati.

```csharp
public Cell this[int row, int column] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| riga | Indice della riga. |
| colonna | Indice colonna. |

### Valore di ritorno

L'oggetto [`Cell`](../../cell/).

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Utilizzo della proprietà Item per accedere e modificare le celle
            cells[0, 0].PutValue("Hello");
            cells[1, 0].PutValue("World");
            
            // Utilizzo della proprietà Style tramite Cells
            Style style1 = cells[0, 0].GetStyle();
            style1.Font.IsBold = true;
            cells[0, 0].SetStyle(style1);

            Style style2 = cells[1, 0].GetStyle();
            style2.Font.Color = System.Drawing.Color.Red;
            cells[1, 0].SetStyle(style2);

            // Salva la cartella di lavoro
            workbook.Save("CellsPropertyItemDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Cells indexer (2 of 2)

Ottiene l'elemento [`Cell`](../../cell/) con il nome della cella specificato.

```csharp
public Cell this[string cellName] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| cellName | Nome della cella, includendo la lettera della colonna e il numero della riga, ad esempio A5. |

### Valore di ritorno

Un oggetto [`Cell`](../../cell/)

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyItemDemo1
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accedi alla raccolta di celle
            Cells cells = worksheet.Cells;
            
            // Imposta i valori utilizzando la proprietà Item
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Age");
            
            // Imposta i valori in un intervallo utilizzando la proprietà Item
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(30);
            cells["A3"].PutValue("Alice");
            cells["B3"].PutValue(25);
            
            // Accedi e modifica le proprietà della cella utilizzando Item
            Cell cell = cells["B1"];
            Style style = cell.GetStyle();
            style.Font.IsBold = true;
            cell.SetStyle(style);
            
            // Salva la cartella di lavoro
            workbook.Save("CellsPropertyItemDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


