---
title: "ImportTableOptions.CheckMergedCells"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ImportTableOptions özelliği. Birleştirilmiş hücrelerin kontrol edilip edilmeyeceğini gösterir"
type: docs
url: /tr/net/aspose.cells/importtableoptions/checkmergedcells/
---
## ImportTableOptions.CheckMergedCells property

Birleştirilmiş hücrelerin kontrol edilip edilmediğini belirtir.

```csharp
public bool CheckMergedCells { get; set; }
```

### Örnekler

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class Customer1
    {
        public int CustomerId { get; set; }
        public string Name { get; set; }
    }

    public class ImportTableOptionsPropertyCheckMergedCellsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Demonstrasyon için birleştirilmiş hücreler oluştur
            worksheet.Cells.Merge(3, 3, 2, 1); // Merge D4:D5
            worksheet.Cells[3, 3].PutValue("MergedValue");

            // Örnek veri oluştur
            List<Customer1> customers = new List<Customer1>
            {
                new Customer1 { CustomerId = 1, Name = "Customer1" },
                new Customer1 { CustomerId = 2, Name = "Customer2" },
                new Customer1 { CustomerId = 3, Name = "Customer3" }
            };

            // CheckMergedCells etkinleştirilmiş şekilde içe aktarma seçeneklerini ayarla
            ImportTableOptions options = new ImportTableOptions
            {
                IsFieldNameShown = false,
                InsertRows = true,
                CheckMergedCells = true
            };

            // Veri içe aktar
            worksheet.Cells.ImportCustomObjects(customers, 0, 0, options);

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx", SaveFormat.Xlsx);

            // Birleştirilmiş hücrelerin korunduğunu doğrula
            Cell mergedCell = worksheet.Cells["D4"];
            Console.WriteLine($"Merged cell value: {mergedCell.StringValue}");
            Console.WriteLine($"Is cell merged: {mergedCell.IsMerged}");
        }
    }
}
```

### Ayrıca Bakınız

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


