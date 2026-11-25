---
title: "Font.Underline"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Font. Ottiene o imposta il tipo di sottolineatura del carattere"
type: docs
url: /it/net/aspose.cells/font/underline/
---
## Font.Underline property

Ottiene o imposta il tipo di sottolineatura del carattere.

```csharp
public FontUnderlineType Underline { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyUnderlineDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Accedi alla cella e imposta lo stile di sottolineatura
            Cell cell = sheet.Cells["A1"];
            cell.PutValue("Sample Underlined Text");
            
            // Ottieni lo stile e modifica le proprietà del carattere
            Style style = cell.GetStyle();
            style.Font.Underline = FontUnderlineType.Single;
            cell.SetStyle(style);

            // Salva la cartella di lavoro
            workbook.Save("FontUnderlineDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [FontUnderlineType](../../fontunderlinetype/)
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


