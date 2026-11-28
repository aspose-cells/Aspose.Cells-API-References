---
title: "PivotTable.GetCellByDisplayName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTable yöntemi. PivotField'ın görüntüleme adıyla Cell nesnesini alır"
type: docs
url: /tr/net/aspose.cells.pivot/pivottable/getcellbydisplayname/
---
## PivotTable.GetCellByDisplayName method

PivotField'ın görüntüleme adıyla [`Cell`](../../../aspose.cells/cell/) nesnesini alır.

```csharp
public Cell GetCellByDisplayName(string displayName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| displayName | String | PivotField'ın DisplayName'i |

### Dönüş Değeri

Cell nesnesi

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodGetCellByDisplayNameWithStringDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Özet tablo için örnek veri ekle
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;

            // Özet tablo oluştur
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Satır alanı ve veri alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Özet tabloyu yenile ve hesapla
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Veri alanının görüntüleme adını al
            string displayName = pivotTable.DataFields[0].DisplayName;

            // GetCellByDisplayName yöntemini kullan
            Cell cell = pivotTable.GetCellByDisplayName(displayName);

            // Sonuçları çıktı olarak ver
            Console.WriteLine("Display Name: " + displayName);
            Console.WriteLine("Cell Name: " + (cell != null ? cell.Name : "null"));
            Console.WriteLine("Cell Value: " + (cell != null ? cell.Value.ToString() : "null"));

            // Çalışma kitabını kaydedin
            workbook.Save("PivotTable_GetCellByDisplayName_Output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../../../aspose.cells/cell/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


