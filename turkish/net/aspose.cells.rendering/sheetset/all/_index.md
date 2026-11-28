---
title: "SheetSet.All"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SheetSet özelliği. Çalışma kitabının tüm sayfalarını orijinal sırasıyla içeren bir küme alır"
type: docs
url: /tr/net/aspose.cells.rendering/sheetset/all/
---
## SheetSet.All property

Çalışma kitabının tüm sayfalarını orijinal sıralarında içeren bir set alır.

```csharp
public static SheetSet All { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetSetPropertyAllDemo
    {
        public static void Run()
        {
            // İki çalışma sayfası içeren bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // Her iki sayfada da örnek veri ayarlayın
            workbook.Worksheets[0].Cells["A1"].PutValue("Sheet1 Data");
            workbook.Worksheets[1].Cells["A1"].PutValue("Sheet2 Data");

            // Tüm sayfaları markdown'a kaydet
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();
            saveOptions.SheetSet = SheetSet.All;
            
            workbook.Save("output.md", saveOptions);
            Console.WriteLine("All sheets saved to markdown successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


