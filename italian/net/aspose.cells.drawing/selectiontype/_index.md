---
title: "Enum SelectionType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.SelectionType enum. Il tipo di selezione della casella di riepilogo"
type: docs
url: /it/net/aspose.cells.drawing/selectiontype/
---
## SelectionType enumeration

Il tipo di selezione della casella di riepilogo.

```csharp
public enum SelectionType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Single | `0` | Tipo di selezione singola. |
| Multi | `1` | Tipo di selezione multipla. |
| Extend | `2` | Estendi il tipo di selezione. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassSelectionTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una casella di riepilogo al foglio di lavoro
            ListBox listBox = worksheet.Shapes.AddListBox(1, 0, 1, 1, 5, 10);

            // Imposta il tipo di selezione su Singola
            listBox.SelectionType = SelectionType.Single;

            // Aggiungi elementi alla casella di riepilogo
            listBox.SetInputRange("A1:A5", false, false);

            // Verifica il tipo di selezione
            Console.WriteLine("ListBox SelectionType: " + listBox.SelectionType);

            // Salva la cartella di lavoro
            workbook.Save("SelectionTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


