---
title: "FileFontSource.FilePath"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FileFontSource. Percorso al file del font"
type: docs
url: /it/net/aspose.cells/filefontsource/filepath/
---
## FileFontSource.FilePath property

Percorso del file di font.

```csharp
public string FilePath { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFontSourcePropertyFilePathDemo
    {
        public static void Run()
        {
            string fontFilePath = "C:\\Fonts\\CustomFont.ttf";
            FileFontSource fontSource = new FileFontSource(fontFilePath);

            Console.WriteLine("Font File Path: " + fontSource.FilePath);

            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            Cell cell = sheet.Cells["A1"];
            cell.PutValue("Test with custom font");

            Style style = cell.GetStyle();
            style.Font.Name = "CustomFont";
            cell.SetStyle(style);

            workbook.Save("FileFontSourceExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [FileFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


