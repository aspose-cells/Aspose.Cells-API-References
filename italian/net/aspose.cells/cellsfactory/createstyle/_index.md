---
title: "CellsFactory.CreateStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo CellsFactory. Crea un nuovo stile"
type: docs
url: /it/net/aspose.cells/cellsfactory/createstyle/
---
## CellsFactory.CreateStyle method

Crea un nuovo stile.

```csharp
public Style CreateStyle()
```

### Valore di ritorno

Restituisce un oggetto stile.

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellsFactoryMethodCreateStyleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Crea uno stile usando CellsFactory
            Style style = new CellsFactory().CreateStyle();
            
            // Imposta le proprietà del bordo per lo stile
            style.SetBorder(BorderType.BottomBorder, CellBorderType.Thick, Color.Black);
            
            // Applica lo stile a una cella
            workbook.Worksheets[0].Cells["A1"].Value = "Hello World";
            workbook.Worksheets[0].Cells["A1"].SetStyle(style);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Style](../../style/)
* class [CellsFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


