---
title: "Worksheet.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Worksheet. Rappresenta il tipo di foglio di lavoro"
type: docs
url: /it/net/aspose.cells/worksheet/type/
---
## Worksheet.Type property

Rappresenta il tipo di foglio di lavoro.

```csharp
public SheetType Type { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta alcune proprietà di base
            worksheet.Name = "DemoSheet";
            worksheet.IsVisible = true;
            
            // Dimostra l'uso della proprietà Type
            Console.WriteLine("Worksheet Type: " + worksheet.Type);
            
            // Aggiungi un foglio grafico per dimostrare diversi tipi di foglio di lavoro
            workbook.Worksheets.Add(SheetType.Chart);
            Worksheet chartSheet = workbook.Worksheets[1];
            
            // Confronta i tipi di foglio di lavoro
            Console.WriteLine("Regular Sheet Type: " + worksheet.Type);
            Console.WriteLine("Chart Sheet Type: " + chartSheet.Type);
            
            // Salva la cartella di lavoro
            workbook.Save("WorksheetTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [SheetType](../../sheettype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


