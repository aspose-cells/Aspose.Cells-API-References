---
title: "FileFontSource.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FileFontSource. Restituisce il tipo della sorgente del font"
type: docs
url: /it/net/aspose.cells/filefontsource/type/
---
## FileFontSource.Type property

Restituisce il tipo della fonte del font.

```csharp
public override FontSourceType Type { get; }
```

### Esempi

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
            
            // Crea un'istanza di FileFontSource
            FileFontSource fontSource = new FileFontSource(fontFilePath);
            
            // Dimostra l'uso della proprietà Type
            Console.WriteLine("Font Source Type: " + fontSource.Type);
            
            // Crea cartella di lavoro e applica il font
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

### Vedi anche

* enum [FontSourceType](../../fontsourcetype/)
* class [FileFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


