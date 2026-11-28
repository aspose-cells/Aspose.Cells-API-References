---
title: "PivotTable.CustomListSort"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTable özelliği. Veri sıralanırken yerleşik özel listenin dikkate alınıp alınmayacağını gösterir"
type: docs
url: /tr/net/aspose.cells.pivot/pivottable/customlistsort/
---
## PivotTable.CustomListSort property

Veri sıralanırken yerleşik özel listenin dikkate alınıp alınmayacağını belirtir.

```csharp
public bool CustomListSort { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyCustomListSortDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Özet tablo için örnek veri ekle
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 20;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 15;
            cells["A5"].Value = "Pear";
            cells["B5"].Value = 5;

            // Özet tablo oluştur
            int index = sheet.PivotTables.Add("A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Satır alanı ve veri alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Özel liste sıralamayı etkinleştir
            pivotTable.CustomListSort = true;

            // Çalışma kitabını kaydedin
            workbook.Save("PivotTable_CustomListSort_Example.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


