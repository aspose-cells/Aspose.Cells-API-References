---
title: "CheckBoxCollection.Add"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo CheckBoxCollection. Aggiunge un checkBox alla collezione"
type: docs
url: /it/net/aspose.cells.drawing/checkboxcollection/add/
---
## CheckBoxCollection.Add method

Aggiunge un checkBox alla collezione.

```csharp
public int Add(int topRow, int leftColumn, int height, int width)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | Int32 | Indice della riga in alto a sinistra. |
| leftColumn | Int32 | Indice della colonna in alto a sinistra. |
| altezza | Int32 | Altezza del checkBox, in unità di pixel. |
| larghezza | Int32 | Larghezza del checkBox, in unità di pixel. |

### Valore di ritorno

[`CheckBox`](../../checkbox/) object index.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class CheckBoxCollectionMethodAddWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un checkbox usando parametri Int32 (upperLeftRow, upperLeftColumn, height, width)
            int index = worksheet.CheckBoxes.Add(10, 2, 20, 100);
            
            CheckBox checkBox = worksheet.CheckBoxes[index];
            checkBox.Text = "Sample CheckBox";
            checkBox.Value = true;
            checkBox.LinkedCell = "B11";
            
            workbook.Save("CheckBoxDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [CheckBoxCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


