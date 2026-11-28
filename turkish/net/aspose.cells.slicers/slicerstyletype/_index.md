---
title: "Enum SlicerStyleType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Slicers.SlicerStyleType enum. Dilimleyici görünümünün stilini belirtin"
type: docs
url: /tr/net/aspose.cells.slicers/slicerstyletype/
---
## SlicerStyleType enumeration

Dilimleyici görünümünün stilini belirtin

```csharp
public enum SlicerStyleType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| SlicerStyleLight1 | `0` | yerleşik açık stil bir |
| SlicerStyleLight2 | `1` | yerleşik açık stil iki |
| SlicerStyleLight3 | `2` | yerleşik açık stil üç |
| SlicerStyleLight4 | `3` | yerleşik açık stil dört |
| SlicerStyleLight5 | `4` | yerleşik açık stil beş |
| SlicerStyleLight6 | `5` | yerleşik açık stil altı |
| SlicerStyleOther1 | `6` | yerleşik stil diğer bir |
| SlicerStyleOther2 | `7` | yerleşik stil diğer iki |
| SlicerStyleDark1 | `8` | yerleşik koyu stil bir |
| SlicerStyleDark2 | `9` | yerleşik koyu stil iki |
| SlicerStyleDark3 | `10` | yerleşik koyu stil üç |
| SlicerStyleDark4 | `11` | yerleşik koyu stil dört |
| SlicerStyleDark5 | `12` | yerleşik koyu stil beş |
| SlicerStyleDark6 | `13` | yerleşik koyu stil altı |
| Custom | `14` | kullanıcı tanımlı stil, şu anda desteklenmiyor |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicersClassSlicerStyleTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // Özet tablo için örnek veri oluştur
            sheet.Cells["A1"].Value = "Fruit";
            sheet.Cells["A2"].Value = "Apple";
            sheet.Cells["A3"].Value = "Orange";
            sheet.Cells["A4"].Value = "Banana";
            sheet.Cells["A5"].Value = "Apple";
            sheet.Cells["B1"].Value = "Quantity";
            sheet.Cells["B2"].Value = 10;
            sheet.Cells["B3"].Value = 15;
            sheet.Cells["B4"].Value = 8;
            sheet.Cells["B5"].Value = 12;

            // Özet tablo oluştur
            int pivotIndex = sheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            pivot.AddFieldToArea(PivotFieldType.Data, 1);

            // Slicer ekle
            int slicerIndex = sheet.Slicers.Add(pivot, "G1", pivot.BaseFields[0]);
            Slicer slicer = sheet.Slicers[slicerIndex];
            
            // Dilimleyici stilini ayarla
            slicer.StyleType = SlicerStyleType.SlicerStyleDark1;
            slicer.NumberOfColumns = 2;

            // Çalışma kitabını kaydedin
            wb.Save("SlicerStyleTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Slicers](../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../)


