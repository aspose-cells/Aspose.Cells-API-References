---
title: "CopyOptions.ColumnCharacterWidth"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CopyOptions özelliği. Karakter biriminde sütun genişliğini kopyalayıp kopyalamayacağını gösterir"
type: docs
url: /tr/net/aspose.cells/copyoptions/columncharacterwidth/
---
## CopyOptions.ColumnCharacterWidth property

Sütun genişliğinin karakter biriminde kopyalanıp kopyalanmayacağını gösterir.

```csharp
public bool ColumnCharacterWidth { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyColumnCharacterWidthDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir kaynak çalışma kitabı oluştur
            Workbook srcWorkbook = new Workbook();
            Worksheet srcSheet = srcWorkbook.Worksheets[0];
            
            // Gösterim için sütun genişliğini karakter cinsinden ayarla
            srcSheet.Cells.SetColumnWidth(0, 20); // 20 characters wide
            
            // Örnek veri ekleyin
            srcSheet.Cells["A1"].PutValue("Sample Text");
            srcSheet.Cells["A2"].PutValue("Another Sample");
            
            // Hedef çalışma kitabı oluştur
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];
            
            // ColumnCharacterWidth true olarak ayarlandığında kopyala
            destSheet.Copy(srcSheet, new CopyOptions()
            {
                ColumnCharacterWidth = true
            });
            
            // Sonucu kaydet
            destWorkbook.Save("output_with_column_width.xlsx", SaveFormat.Xlsx);
            
            // Karşılaştırma için, ColumnCharacterWidth olmadan kopyala
            Workbook destWorkbook2 = new Workbook();
            Worksheet destSheet2 = destWorkbook2.Worksheets[0];
            
            destSheet2.Copy(srcSheet, new CopyOptions()
            {
                ColumnCharacterWidth = false
            });
            
            destWorkbook2.Save("output_without_column_width.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


