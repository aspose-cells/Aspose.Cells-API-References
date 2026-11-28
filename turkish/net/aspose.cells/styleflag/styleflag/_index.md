---
title: "StyleFlag.StyleFlag"
second_title: "Aspose.Cells için .NET API Referansı"
description: "StyleFlag yapıcı. Tüm bayrakların false olduğu bir nesne oluşturur"
type: docs
url: /tr/net/aspose.cells/styleflag/styleflag/
---
## StyleFlag constructor

Tüm bayrakları false olarak ayarlayan bir nesne oluşturur.

```csharp
public StyleFlag()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagMethodCtorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Kalın bir stil oluştur
            Style boldStyle = workbook.CreateStyle();
            boldStyle.Font.IsBold = true;

            // StyleFlag yapıcı ile 9. satıra stili uygula
            worksheet.Cells.ApplyRowStyle(9, boldStyle, new StyleFlag { FontBold = true });

            // Hücreye değer koyun ve stili doğrulayın
            worksheet.Cells[9, 0].PutValue("Bold Text");

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");

            Console.WriteLine("Style applied successfully using StyleFlag constructor.");
        }
    }
}
```

### Ayrıca Bakınız

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


