---
title: "FileFontSource.FileFontSource"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор FileFontSource. Ctor"
type: docs
url: /ru/net/aspose.cells/filefontsource/filefontsource/
---
## FileFontSource constructor

Конструктор.

```csharp
public FileFontSource(string filePath)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| filePath | String | путь к файлу шрифта |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFontSourceMethodCtorWithStringDemo
    {
        public static void Run()
        {
            string fontFilePath = "C:\\Fonts\\CustomFont.ttf";
            FileFontSource fontSource = new FileFontSource(fontFilePath);

            Console.WriteLine("Font Source Type: " + fontSource.Type);
            Console.WriteLine("Font File Path: " + fontSource.FilePath);

            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            Cell cell = sheet.Cells["A1"];
            cell.PutValue("Sample Text");

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


