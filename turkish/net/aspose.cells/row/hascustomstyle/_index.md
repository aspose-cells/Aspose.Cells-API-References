---
title: "Row.HasCustomStyle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Satır özelliği. Bu satırın, çalışma kitabından devralınan varsayılan stilden farklı özel stil ayarlarına sahip olup olmadığını gösterir."
type: docs
url: /tr/net/aspose.cells/row/hascustomstyle/
---
## Row.HasCustomStyle property

Bu satırın özel stil ayarları (varsayılan ayardan ve çalışma kitabından devralınanından farklı) olup olmadığını gösterir.

```csharp
public bool HasCustomStyle { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RowPropertyHasCustomStyleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bir stil oluşturun ve özelleştirin
            Style customStyle = workbook.CreateStyle();
            customStyle.BackgroundColor = Color.LightBlue;
            customStyle.Pattern = BackgroundType.Solid;
            
            // İlk satıra erişin
            Row row = worksheet.Cells.Rows[0];
            
            // Satıra özel stil uygulayın
            row.ApplyStyle(customStyle, new StyleFlag { All = true });
            
            // Satırın özel stiline sahip olup olmadığını kontrol edin (doğru olmalı)
            bool hasCustomStyle = row.HasCustomStyle;
            Console.WriteLine("Row has custom style: " + hasCustomStyle);
            
            // Çalışma kitabını kaydedin
            workbook.Save("RowHasCustomStyleDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


