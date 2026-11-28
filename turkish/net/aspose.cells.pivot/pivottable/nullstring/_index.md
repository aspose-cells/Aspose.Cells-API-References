---
title: "PivotTable.NullString"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTable özelliği. DisplayNullString özelliği true olduğunda null değer içeren hücrelerde gösterilen dizeyi alır. Varsayılan değer boş bir dizedir."
type: docs
url: /tr/net/aspose.cells.pivot/pivottable/nullstring/
---
## PivotTable.NullString property

DisplayNullString özelliği true olduğunda null değer içeren hücrelerde gösterilen dizeyi alır. Varsayılan değer boş bir dizedir.

```csharp
public string NullString { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyNullStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Özet tablo için örnek veri ekle
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 2000;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 3000;
            cells["A5"].Value = null; // Null value
            cells["B5"].Value = 4000;

            // Özet tablo oluştur
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Pivot tabloya alan ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // NullString özelliğini ve görüntüleme ayarlarını ayarla
            pivotTable.NullString = "(null)";
            pivotTable.DisplayNullString = true;

            // Özet tablo verilerini yenile
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Çalışma kitabını kaydedin
            workbook.Save("PivotTableNullStringDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


