---
title: "Font.IsItalic"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Font. Ottiene o imposta un valore che indica se il carattere è in corsivo"
type: docs
url: /it/net/aspose.cells/font/isitalic/
---
## Font.IsItalic property

Ottiene o imposta un valore che indica se il carattere è in corsivo.

```csharp
public bool IsItalic { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyIsItalicDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi allo stile predefinito
            Style style = workbook.DefaultStyle;
            
            // Imposta le proprietà del carattere includendo IsItalic
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.Font.IsItalic = true;
            
            // Applica lo stile alla cella A1
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            cell.PutValue("Italic Text Example");
            
            // Salva la cartella di lavoro
            workbook.Save("FontPropertyIsItalicDemo.xlsx");
            
            // Verifica la proprietà corsivo
            Console.WriteLine("Font is italic: " + cell.GetStyle().Font.IsItalic);
        }
    }
}
```

### Vedi anche

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


