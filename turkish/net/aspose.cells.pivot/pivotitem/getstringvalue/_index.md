---
title: "PivotItem.GetStringValue"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotItem yöntemi. Pivot öğesinin dize değerini alır. Değer null ise döndürür"
type: docs
url: /tr/net/aspose.cells.pivot/pivotitem/getstringvalue/
---
## PivotItem.GetStringValue method

Pivot öğesinin metin değerini alır. Değer null ise, "" döndürür.

```csharp
public string GetStringValue()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemMethodGetStringValueDemo
    {
        public static void Run()
        {
            // Kaynak Excel dosyasından bir çalışma kitabı oluştur
            Workbook workbook = new Workbook("example.xlsx");
            
            // İlk çalışma sayfasına ve pivot tabloya erişin
            Worksheet worksheet = workbook.Worksheets[0];
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // İlk satır alanını ve onun pivot öğelerini alın
            PivotField rowField = pivotTable.RowFields[0];
            PivotItemCollection pivotItems = rowField.PivotItems;
            
            // GetStringValue() yöntemini gösterin
            string itemValue = pivotItems[1].GetStringValue();
            Console.WriteLine("PivotItem value: " + itemValue);
            
            // Değiştirilmiş çalışma kitabını kaydet
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


