---
title: "FileFontSource.FileFontSource"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FileFontSource yapıcı. Ctor"
type: docs
url: /tr/net/aspose.cells/filefontsource/filefontsource/
---
## FileFontSource constructor

Yapıcı.

```csharp
public FileFontSource(string filePath)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| filePath | String | yazı tipi dosyasının yolu |

### Örnekler

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

### Ayrıca Bakınız

* class [FileFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


