---
title: "PivotTable.DataFields"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTable özelliği. Bir PivotTable'daki tüm veri alanlarını temsil eden bir PivotFieldCollection döndürür"
type: docs
url: /tr/net/aspose.cells.pivot/pivottable/datafields/
---
## PivotTable.DataFields property

Bir PivotTable'daki tüm veri alanlarını temsil eden bir [`PivotFieldCollection`](../../pivotfieldcollection/) döndürür.

```csharp
public PivotFieldCollection DataFields { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyDataFieldsDemo
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

            // Bir pivot tablo ekle
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Satır alanı ve veri alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Veri alanlarına erişin ve işlevselliği gösterin
            PivotFieldCollection dataFields = pivotTable.DataFields;
            if (dataFields.Count > 0)
            {
                PivotField dataField = dataFields[0];
                Console.WriteLine("Data Field Name: " + dataField.Name);
                Console.WriteLine("Data Field Function: " + dataField.Function);
            }

            // Çalışma kitabını kaydedin
            workbook.Save("PivotTableDataFieldsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotFieldCollection](../../pivotfieldcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


