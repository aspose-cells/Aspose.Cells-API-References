---
title: "Font.IsBold"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Font. Ottiene o imposta un valore che indica se il carattere è in grassetto"
type: docs
url: /it/net/aspose.cells/font/isbold/
---
## Font.IsBold property

Ottiene o imposta un valore che indica se il carattere è in grassetto.

```csharp
public bool IsBold { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyIsBoldDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accedi alla cella A1 e imposta il suo valore
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Bold Text Demo");
            
            // Ottieni lo stile della cella e imposta il carattere in grassetto
            Style style = cell.GetStyle();
            style.Font.IsBold = true;
            cell.SetStyle(style);
            
            // Salva la cartella di lavoro
            workbook.Save("FontIsBoldDemo.xlsx");
            
            // Verifica la proprietà grassetto
            Workbook loadedWorkbook = new Workbook("FontIsBoldDemo.xlsx");
            Style loadedStyle = loadedWorkbook.Worksheets[0].Cells["A1"].GetStyle();
            Console.WriteLine("IsBold property: " + loadedStyle.Font.IsBold);
        }
    }
}
```

### Vedi anche

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


