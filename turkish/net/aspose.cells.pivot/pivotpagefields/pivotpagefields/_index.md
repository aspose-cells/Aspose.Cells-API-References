---
title: "PivotPageFields.PivotPageFields"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotPageFields yapıcı. Pivot sayfa alanı öğelerini temsil eder"
type: docs
url: /tr/net/aspose.cells.pivot/pivotpagefields/pivotpagefields/
---
## PivotPageFields constructor

Pivot sayfa alanı öğelerini temsil eder.

```csharp
public PivotPageFields()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotPageFieldsMethodSharpctorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Özet tablo için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Region");
            worksheet.Cells["C1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue("East");
            worksheet.Cells["C2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue("West");
            worksheet.Cells["C3"].PutValue(2000);

            // Yapıcıyı kullanarak pivot sayfa alanları oluştur
            PivotPageFields pageFields = new PivotPageFields();
            
            // Sayfa alanları ekle
            string[] items = { "Item1", "Item2" };
            pageFields.AddPageField(items);
            
            // Tanımlama ekle
            int[] itemIndexes = { 0, 1 };
            pageFields.AddIdentify(0, itemIndexes);

            // Doğru parametrelerle pivot tablo ekle
            PivotTableCollection pivotTables = worksheet.PivotTables;
            string sourceData = "A1:C3";
            int index = pivotTables.Add(sourceData, "E5", "PivotTable1");

            // Çalışma kitabını kaydedin
            workbook.Save("PivotPageFieldsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotPageFields](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


