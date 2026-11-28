---
title: "Worksheet.Workbook"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet özelliği. Bu sayfayı içeren çalışma kitabı nesnesini alır"
type: docs
url: /tr/net/aspose.cells/worksheet/workbook/
---
## Worksheet.Workbook property

Bu sayfayı içeren çalışma kitabı nesnesini alır.

```csharp
public Workbook Workbook { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyWorkbookDemo
    {
        public static void Run()
        {
            // Bir kaynak çalışma kitabı oluştur ve bir çalışma sayfası al
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            
            // Kaynak çalışma sayfasına örnek veri ekle
            sourceSheet.Cells["A1"].PutValue("Sample Data");
            sourceSheet.Cells["A2"].PutValue(100);
            sourceSheet.Cells["A3"].PutValue(200);
            
            // Bir hedef çalışma kitabı oluştur
            Workbook destWorkbook = new Workbook();
            
            // Worksheet.Workbook özelliğini kullanarak kaynak çalışma kitabından temayı kopyala
            destWorkbook.CopyTheme(sourceSheet.Workbook);
            
            // Hedef çalışma sayfasına eriş ve verileri kopyala
            Worksheet destSheet = destWorkbook.Worksheets[0];
            Aspose.Cells.Range sourceRange = sourceSheet.Cells.CreateRange("A1:A3");
            Aspose.Cells.Range destRange = destSheet.Cells.CreateRange("A1:A3");
            
            // Verileri biçimlendirme ile kopyala
            destRange.Copy(sourceRange);
            
            // Hedef çalışma kitabını kaydet
            destWorkbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../../workbook/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


