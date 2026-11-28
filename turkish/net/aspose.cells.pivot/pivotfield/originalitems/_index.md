---
title: "PivotField.OriginalItems"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotField özelliği. Orijinal temel öğeleri al"
type: docs
url: /tr/net/aspose.cells.pivot/pivotfield/originalitems/
---
## PivotField.OriginalItems property

Orijinal temel öğeleri al;

```csharp
public string[] OriginalItems { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyOriginalItemsDemo
    {
        public static void Run()
        {
            // Kaynak Excel dosyasından bir çalışma kitabı oluştur
            Workbook workbook = new Workbook("AsposeGroupedField2.xlsx");
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // İlk pivot tabloya eriş
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // İlk satır alanına eriş
            PivotField pivotField = pivotTable.RowFields[0];
            
            // Orijinal öğeleri ve gruplanmış öğeleri göster
            Console.WriteLine("Original Item[0]: " + pivotField.OriginalItems[0]);
            Console.WriteLine("Grouped Item[0]: " + pivotField.Items[0]);
            
            // Değiştirilmiş çalışma kitabını kaydet
            workbook.Save("PivotFieldOriginalItemsDemo_Output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


