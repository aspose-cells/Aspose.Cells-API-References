---
title: "Row.HasCustomStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Row proprietà. Indica se questa riga ha impostazioni di stile personalizzate diverse dallo stile predefinito ereditato dalla cartella di lavoro"
type: docs
url: /it/net/aspose.cells/row/hascustomstyle/
---
## Row.HasCustomStyle property

Indica se questa riga ha impostazioni di stile personalizzate (diverse da quelle predefinite ereditate dalla cartella di lavoro).

```csharp
public bool HasCustomStyle { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RowPropertyHasCustomStyleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea e personalizza uno stile
            Style customStyle = workbook.CreateStyle();
            customStyle.BackgroundColor = Color.LightBlue;
            customStyle.Pattern = BackgroundType.Solid;
            
            // Accedi alla prima riga
            Row row = worksheet.Cells.Rows[0];
            
            // Applica lo stile personalizzato alla riga
            row.ApplyStyle(customStyle, new StyleFlag { All = true });
            
            // Verifica se la riga ha uno stile personalizzato (dovrebbe essere vero)
            bool hasCustomStyle = row.HasCustomStyle;
            Console.WriteLine("Row has custom style: " + hasCustomStyle);
            
            // Salva la cartella di lavoro
            workbook.Save("RowHasCustomStyleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


