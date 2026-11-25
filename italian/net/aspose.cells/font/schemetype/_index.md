---
title: "Font.SchemeType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Font. Ottiene e imposta il tipo di schema del Font"
type: docs
url: /it/net/aspose.cells/font/schemetype/
---
## Font.SchemeType property

Ottiene e imposta il tipo di schema del carattere.

```csharp
public FontSchemeType SchemeType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertySchemeTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");

            Font font = cell.GetStyle().Font;
            font.SchemeType = FontSchemeType.Minor;
            font.Name = "Calibri";
            font.Size = 12;

            workbook.Save("FontSchemeTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [FontSchemeType](../../fontschemetype/)
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


