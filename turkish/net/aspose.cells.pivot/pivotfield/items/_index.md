---
title: "PivotField.Items"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotField özelliği. Bu alandaki pivot öğelerinin tüm etiketlerini al"
type: docs
url: /tr/net/aspose.cells.pivot/pivotfield/items/
---
## PivotField.Items property

Bu alandaki pivot öğelerinin tüm etiketlerini al.

```csharp
public string[] Items { get; }
```

### Örnekler

```csharp
using System;
using System.Collections;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyItemsDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluşturun ve örnek veri ekleyin
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Özet tablo için örnek veri ekle
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["A5"].Value = "Apple";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 15;
            worksheet.Cells["B4"].Value = 20;
            worksheet.Cells["B5"].Value = 5;

            // Özet tablo oluştur
            int index = worksheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Pivot alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            PivotField pivotField = pivotTable.RowFields[0];
            
            // Items özelliğini göster
            string[] items = pivotField.Items;
            Console.WriteLine("Pivot Field Items:");
            foreach (string item in items)
            {
                Console.WriteLine(item);
            }
            
            // Geçerli sayfa öğesini ayarla
            ArrayList list = new ArrayList(items);
            if (list.Contains("Apple"))
            {
                pivotField.CurrentPageItem = (short)list.IndexOf("Apple");
                Console.WriteLine("Current page item set to: Apple");
            }
            
            pivotTable.CalculateData();
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


