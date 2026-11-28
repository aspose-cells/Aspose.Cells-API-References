---
title: "Protection.AllowUsingPivotTable"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Protection özelliği. Kullanıcının korumalı bir çalışma sayfasında pivot tablolarını manipüle etmesine izin verilip verilmediğini temsil eder."
type: docs
url: /tr/net/aspose.cells/protection/allowusingpivottable/
---
## Protection.AllowUsingPivotTable property

Korunan bir çalışma sayfasında özet tabloyu manipüle etme izni olup olmadığını temsil eder.

```csharp
public bool AllowUsingPivotTable { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowUsingPivotTableDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfası korumasını etkinleştir
            Protection protection = worksheet.Protection;
            protection.AllowUsingPivotTable = true;
            worksheet.Protect(ProtectionType.All);

            // Ayarı doğrula
            Console.WriteLine("AllowUsingPivotTable is set to: " + protection.AllowUsingPivotTable);

            // İşlevselliği göstermek için bir pivot tablo oluşturun.
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(150);

            // Doğru parametrelerle pivot tablo oluşturun.
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "C1", "PivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Çalışma kitabını kaydedin
            workbook.Save("ProtectionPropertyAllowUsingPivotTableDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


