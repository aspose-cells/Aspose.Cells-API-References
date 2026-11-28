---
title: "PivotFieldCollection.Type"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotFieldCollection özelliği. PivotFields tipini alır"
type: docs
url: /tr/net/aspose.cells.pivot/pivotfieldcollection/type/
---
## PivotFieldCollection.Type property

PivotFields tipini alır.

```csharp
public PivotFieldType Type { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldCollectionPropertyTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Pivot tablo için örnek veri ekle
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B3"].Value = 5;
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B4"].Value = 7;

            // Bir pivot tablo oluştur
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Satır alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            PivotFieldCollection rowFields = pivotTable.RowFields;

            // Pivot alan koleksiyonunun tipini göster
            Console.WriteLine("PivotFieldCollection Type: " + rowFields.Type);

            // Veri alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            PivotFieldCollection dataFields = pivotTable.DataFields;

            // Veri alan koleksiyonunun tipini göster
            Console.WriteLine("DataFields Type: " + dataFields.Type);

            // Verileri hesapla ve pivot tabloyu yenile
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Sonucu kaydet
            workbook.Save("PivotFieldCollectionTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


