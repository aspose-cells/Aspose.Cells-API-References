---
title: "ShapeCollection.AddListBox"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ShapeCollection. Aggiunge un ListBox al foglio di lavoro."
type: docs
url: /it/net/aspose.cells.drawing/shapecollection/addlistbox/
---
## ShapeCollection.AddListBox method

Aggiunge un ListBox al foglio di lavoro.

```csharp
public ListBox AddListBox(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | Int32 | Indice della riga in alto a sinistra. |
| alto | Int32 | Rappresenta lo spostamento verticale del ListBox dalla sua riga sinistra, in unità di pixel. |
| leftColumn | Int32 | Indice della colonna in alto a sinistra. |
| sinistra | Int32 | Rappresenta lo spostamento orizzontale del ListBox dalla sua colonna sinistra, in unità di pixel. |
| altezza | Int32 | Rappresenta l'altezza del ListBox, in unità di pixel. |
| larghezza | Int32 | Rappresenta la larghezza del ListBox, in unità di pixel. |

### Valore di ritorno

Un oggetto ListBox.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddListBoxWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una casella di riepilogo al foglio di lavoro
            Aspose.Cells.Drawing.ListBox listBox = worksheet.Shapes.AddListBox(1, 0, 1, 0, 100, 50);

            // Aggiungi elementi alla casella di riepilogo
            listBox.SetInputRange("A1:A3", false, false);
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");

            // Salva la cartella di lavoro
            workbook.Save("ListBoxDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ListBox](../../listbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


