---
title: "PivotTable.GrandTotalName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTable özelliği. Genel toplam sütununda veya satır başlığında görüntülenen etiketi döndürür. Varsayılan değer 'Grand Total' dizesidir."
type: docs
url: /tr/net/aspose.cells.pivot/pivottable/grandtotalname/
---
## PivotTable.GrandTotalName property

Grand total sütun veya satır başlığında gösterilen etiketi döndürür. Varsayılan değer "Grand Total" dizesidir.

```csharp
public string GrandTotalName { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyGrandTotalNameDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Pivot tablo için örnek veri ekle
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Region";
            worksheet.Cells["C1"].Value = "Sales";
            
            worksheet.Cells["A2"].Value = "Laptop";
            worksheet.Cells["B2"].Value = "North";
            worksheet.Cells["C2"].Value = 1000;
            
            worksheet.Cells["A3"].Value = "Laptop";
            worksheet.Cells["B3"].Value = "South";
            worksheet.Cells["C3"].Value = 1500;
            
            worksheet.Cells["A4"].Value = "Phone";
            worksheet.Cells["B4"].Value = "North";
            worksheet.Cells["C4"].Value = 800;
            
            worksheet.Cells["A5"].Value = "Phone";
            worksheet.Cells["B5"].Value = "South";
            worksheet.Cells["C5"].Value = 1200;

            // Bir pivot tablo oluştur
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Satır ve veri alanları ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Geçerli GrandTotalName değerini göster
            Console.WriteLine("Current GrandTotalName: " + pivotTable.GrandTotalName);

            // GrandTotalName'i değiştir
            pivotTable.GrandTotalName = "Total Summary";

            // Verileri hesapla ve pivot tabloyu yenile
            pivotTable.CalculateData();
            pivotTable.RefreshData();

            // Çalışma kitabını kaydedin
            workbook.Save("PivotTableGrandTotalNameDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


