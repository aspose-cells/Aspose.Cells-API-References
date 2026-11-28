---
title: "FileFontSource.Type"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FileFontSource özelliği. Yazı tipi kaynağının türünü döndürür"
type: docs
url: /tr/net/aspose.cells/filefontsource/type/
---
## FileFontSource.Type property

Yazı tipi kaynağının türünü döndürür.

```csharp
public override FontSourceType Type { get; }
```

### Örnekler

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
            
            // FileFontSource örneği oluşturun
            FileFontSource fontSource = new FileFontSource(fontFilePath);
            
            // Type özelliğinin kullanımını gösterin.
            Console.WriteLine("Font Source Type: " + fontSource.Type);
            
            // Çalışma kitabı oluştur ve yazı tipini uygula
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

### Ayrıca Bakınız

* enum [FontSourceType](../../fontsourcetype/)
* class [FileFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


