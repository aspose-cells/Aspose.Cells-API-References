---
title: "PivotTable.FieldListSortAscending"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTable özelliği. PivotTable'daki alanların alan listesinde varsayılan olmayan bir sırayla sıralanıp sıralanmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.pivot/pivottable/fieldlistsortascending/
---
## PivotTable.FieldListSortAscending property

**PivotTable** içindeki alanların alan listesinde varsayılan olmayan sırayla sıralanıp sıralanmadığını gösterir.

```csharp
public bool FieldListSortAscending { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyFieldListSortAscendingDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Pivot tablo için örnek veri ekle
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["B1"].Value = "Product";
            worksheet.Cells["C1"].Value = "Sales";
            
            worksheet.Cells["A2"].Value = "Electronics";
            worksheet.Cells["B2"].Value = "Laptop";
            worksheet.Cells["C2"].Value = 1200;
            
            worksheet.Cells["A3"].Value = "Electronics";
            worksheet.Cells["B3"].Value = "Phone";
            worksheet.Cells["C3"].Value = 800;
            
            worksheet.Cells["A4"].Value = "Furniture";
            worksheet.Cells["B4"].Value = "Chair";
            worksheet.Cells["C4"].Value = 150;
            
            worksheet.Cells["A5"].Value = "Furniture";
            worksheet.Cells["B5"].Value = "Table";
            worksheet.Cells["C5"].Value = 250;

            // Bir pivot tablo oluştur
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Pivot tabloya alanlar ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Mevcut FieldListSortAscending değerini göster
            Console.WriteLine("Initial FieldListSortAscending: " + pivotTable.FieldListSortAscending);

            // Alan listesini artan sırada göster
            pivotTable.FieldListSortAscending = true;
            Console.WriteLine("FieldListSortAscending set to: " + pivotTable.FieldListSortAscending);

            // Pivot tabloyu yenileyin ve hesaplayın
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Çalışma kitabını kaydedin
            workbook.Save("PivotTableFieldListSortAscendingDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


