---
title: "FileFontSource.FilePath"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FileFontSource. Путь к файлу шрифта"
type: docs
url: /ru/net/aspose.cells/filefontsource/filepath/
---
## FileFontSource.FilePath property

Путь к файлу шрифта.

```csharp
public string FilePath { get; }
```

### Примеры

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

### См. также

* class [FileFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


