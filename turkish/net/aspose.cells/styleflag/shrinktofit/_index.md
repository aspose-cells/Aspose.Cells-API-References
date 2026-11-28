---
title: "StyleFlag.ShrinkToFit"
second_title: "Aspose.Cells için .NET API Referansı"
description: "StyleFlag özelliği. Sığdırmak için küçült ayarı uygulanacak"
type: docs
url: /tr/net/aspose.cells/styleflag/shrinktofit/
---
## StyleFlag.ShrinkToFit property

Sığdırmak için küçültme ayarı uygulanacak.

```csharp
public bool ShrinkToFit { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyShrinkToFitDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Hücreye örnek veri ayarlayın
            cells["A1"].PutValue("This is a long text that needs to fit in the cell");
            
            // Sığdırmak için küçültme etkinleştirilmiş bir stil oluşturun
            Style style = workbook.CreateStyle();
            style.ShrinkToFit = true;
            
            // Stil bayrağı oluşturun ve Sığdırmak için küçültme bayrağını etkinleştirin
            StyleFlag flag = new StyleFlag();
            flag.ShrinkToFit = true;
            
            // Stili hücre aralığına uygulayın (Aspose.Cells.Range'i açıkça kullanarak)
            Aspose.Cells.Range range = cells.CreateRange("A1");
            range.ApplyStyle(style, flag);
            
            // Küçülmeyi göstermek için sütun genişliğini ayarlayın
            worksheet.Cells.SetColumnWidth(0, 10);
            
            // Çalışma kitabını kaydedin
            workbook.Save("ShrinkToFitDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


