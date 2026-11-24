---
title: "FileFontSource.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FileFontSource‑Eigenschaft. Gibt den Typ der Schriftquelle zurück"
type: docs
url: /de/net/aspose.cells/filefontsource/type/
---
## FileFontSource.Type property

Gibt den Typ der Schriftquellen zurück.

```csharp
public override FontSourceType Type { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFontSourcePropertyTypeDemo
    {
        public static void Run()
        {
            string fontFilePath = "CustomFont.ttf";
            
            // Erstelle eine FileFontSource-Instanz
            FileFontSource fontSource = new FileFontSource(fontFilePath);
            
            // Demonstriere die Verwendung der Type‑Eigenschaft
            Console.WriteLine("Font Source Type: " + fontSource.Type);
            
            // Erstelle eine Arbeitsmappe und wende die Schrift an
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            Cell cell = sheet.Cells["A1"];
            cell.PutValue("Text with custom font");
            
            Style style = cell.GetStyle();
            style.Font.Name = "CustomFont";
            cell.SetStyle(style);
            
            workbook.Save("FontSourceDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [FontSourceType](../../fontsourcetype/)
* class [FileFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


