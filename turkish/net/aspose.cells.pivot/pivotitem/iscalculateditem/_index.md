---
title: "PivotItem.IsCalculatedItem"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotItem özelliği. Bu pivot öğesinin hesaplanmış bir formül öğesi olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.pivot/pivotitem/iscalculateditem/
---
## PivotItem.IsCalculatedItem property

Bu pivot öğesinin hesaplanmış bir formül öğesi olup olmadığını gösterir.

```csharp
public bool IsCalculatedItem { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotItemPropertyIsCalculatedItemDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Pivot tablo için örnek veri ekle
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["A5"].Value = "Apple";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 20;
            worksheet.Cells["B4"].Value = 30;
            worksheet.Cells["B5"].Value = 15;

            // Bir pivot tablo oluştur
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Satır alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // Veri alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Pivot tablo verilerini hesapla
            pivotTable.CalculateData();

            // İlk pivot alanından ilk pivot öğesini al
            PivotField pivotField = pivotTable.RowFields[0];
            PivotItem pivotItem = pivotField.PivotItems[0];

            // IsCalculatedItem özelliği değerini göster
            Console.WriteLine("IsCalculatedItem value: " + pivotItem.IsCalculatedItem);

            // Pivot öğesinin hesaplanmış bir öğe olup olmadığını kontrol et
            if (pivotItem.IsCalculatedItem)
            {
                Console.WriteLine("This pivot item is a calculated formula item.");
                Console.WriteLine("Formula: " + pivotItem.GetFormula());
            }
            else
            {
                Console.WriteLine("This pivot item is not a calculated formula item.");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("PivotItemPropertyIsCalculatedItemDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


