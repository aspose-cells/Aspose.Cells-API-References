---
title: "PivotTable.ErrorString"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTable özelliği. DisplayErrorString özelliği true olduğunda hatalı hücrelerde gösterilen dizeyi alır. Varsayılan değer boş bir dizedir."
type: docs
url: /tr/net/aspose.cells.pivot/pivottable/errorstring/
---
## PivotTable.ErrorString property

DisplayErrorString özelliği true olduğunda hatalar içeren hücrelerde gösterilen dizeyi alır. Varsayılan değer boş bir dizedir.

```csharp
public string ErrorString { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyErrorStringDemo
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
            cells["A2"].Value = "Bike";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "Car";
            cells["B3"].Value = 2000;
            cells["A4"].Value = "Bike";
            cells["B4"].Value = 1500;
            cells["A5"].Value = "Car";
            cells["B5"].Value = 1800;

            // Özet tablo oluştur
            int index = sheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // ErrorString özelliğini ayarla
            pivotTable.ErrorString = "Custom Error";
            pivotTable.DisplayErrorString = true;

            // Pivot tabloya alan ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Verileri hesapla ve pivot tabloyu yenile
            pivotTable.CalculateData();
            pivotTable.RefreshData();

            // Çalışma kitabını kaydedin
            workbook.Save("PivotTableErrorStringDemo.xlsx");

            Console.WriteLine("PivotTable with ErrorString property set successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


