---
title: "PivotItem.Value"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotItem özelliği. Pivot öğesinin değerini alır"
type: docs
url: /tr/net/aspose.cells.pivot/pivotitem/value/
---
## PivotItem.Value property

Pivot öğesinin değerini alır

```csharp
public object Value { get; }
```

### Örnekler

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemPropertyValueDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Özet tablo için örnek veri ekle
            var cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;
            cells["A5"].Value = "Apple";
            cells["B5"].Value = 5;

            // Özet tablo oluştur
            int index = sheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Satır alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // Veri alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // Pivot alanını al
            PivotField pivotField = pivotTable.RowFields[0];
            
            // Pivot öğelerini işle
            List<string> valuesToShow = new List<string> { "Apple", "Banana" };
            
            Console.WriteLine("Pivot Items Before Filtering:");
            PrintPivotItems(pivotField);

            // Değer özelliğine göre pivot öğelerini filtrele
            for (int i = 0; i < pivotField.PivotItems.Count; i++)
            {
                PivotItem item = pivotField.PivotItems[i];
                string itemValue = item.Value?.ToString() ?? "";
                
                if (!valuesToShow.Contains(itemValue))
                {
                    item.IsHidden = true;
                }
            }

            Console.WriteLine("\nPivot Items After Filtering:");
            PrintPivotItems(pivotField);
        }

        private static void PrintPivotItems(PivotField pivotField)
        {
            for (int i = 0; i < pivotField.PivotItems.Count; i++)
            {
                PivotItem item = pivotField.PivotItems[i];
                Console.WriteLine($"Name: {item.Name}, Value: {item.Value}, Hidden: {item.IsHidden}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


