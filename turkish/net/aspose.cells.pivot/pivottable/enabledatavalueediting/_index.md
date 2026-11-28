---
title: "PivotTable.EnableDataValueEditing"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTable özelliği. Kullanıcının pivot tablonun veri alanındaki hücreleri düzenleyip düzenleyemeyeceğini belirten bir boolean değer belirtir. Varsayılan değer false'tur"
type: docs
url: /tr/net/aspose.cells.pivot/pivottable/enabledatavalueediting/
---
## PivotTable.EnableDataValueEditing property

Kullanıcının pivottable veri alanındaki hücreleri düzenlemesine izin verilip verilmediğini belirten bir boolean değer belirtir. Varsayılan değer yanlıştır.

```csharp
public bool EnableDataValueEditing { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyEnableDataValueEditingDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Pivot tablo için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Bike");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Car");
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["A4"].PutValue("Bike");
            worksheet.Cells["B4"].PutValue(1500);
            worksheet.Cells["A5"].PutValue("Car");
            worksheet.Cells["B5"].PutValue(3000);

            // Bir pivot tablo ekle
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Satır alanı ve veri alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // EnableDataValueEditing'in geçerli değerini göster
            Console.WriteLine("Current EnableDataValueEditing value: " + pivotTable.EnableDataValueEditing);

            // Veri değerlerinin düzenlenmesini etkinleştir
            pivotTable.EnableDataValueEditing = true;

            // Pivot tabloyu doldurmak için verileri hesapla
            pivotTable.CalculateData();

            // Düzenlemeden önce çalışma kitabını kaydet
            workbook.Save("PivotTableBeforeEdit.xlsx");

            // Artık veri değerlerini doğrudan pivot tabloda düzenleyebiliriz
            // Demonstrasyon amacıyla, veri alanındaki bir hücreyi değiştireceğiz
            Cell dataCell = worksheet.Cells["F5"]; // Assuming this is a data cell
            if (dataCell != null)
            {
                dataCell.PutValue(2500); // Modify the value
            }

            // Düzenlemeden sonra çalışma kitabını kaydet
            workbook.Save("PivotTableAfterEdit.xlsx");

            // Veri değerlerinin düzenlenmesini devre dışı bırak
            pivotTable.EnableDataValueEditing = false;
            Console.WriteLine("EnableDataValueEditing set to: " + pivotTable.EnableDataValueEditing);
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


