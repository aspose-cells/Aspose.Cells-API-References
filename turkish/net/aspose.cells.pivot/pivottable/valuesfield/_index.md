---
title: "PivotTable.ValuesField"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTable özelliği. Bir PivotTable'daki tüm veri alanlarını temsil eden bir PivotField nesnesi alır. Salt okunurdur. Yalnızca Veri bölgesinde iki veya daha fazla veri alanı olduğunda oluşturulur. Varsayılan olarak satır bölgesindedir. PivotTable.AddFieldToArea yöntemiyle satır/sütun bölgesine sürükleyebilirsiniz."
type: docs
url: /tr/net/aspose.cells.pivot/pivottable/valuesfield/
---
## PivotTable.ValuesField property

Bir [`PivotField`](../../pivotfield/) nesnesi alır; bu nesne bir PivotTable'daki tüm veri alanlarını temsil eder. Salt okunurdur. Yalnızca Veri bölgesinde iki veya daha fazla veri alanı olduğunda oluşturulur. Varsayılan olarak satır bölgesindedir. PivotTable.AddFieldToArea() yöntemiyle satır/sütun bölgesine sürükleyebilirsiniz.

```csharp
public PivotField ValuesField { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyValuesFieldDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Pivot tablo için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Region");
            worksheet.Cells["C1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["B2"].PutValue("North");
            worksheet.Cells["C2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B3"].PutValue("South");
            worksheet.Cells["C3"].PutValue(1500);
            worksheet.Cells["A4"].PutValue("Product A");
            worksheet.Cells["B4"].PutValue("South");
            worksheet.Cells["C4"].PutValue(2000);
            worksheet.Cells["A5"].PutValue("Product B");
            worksheet.Cells["B5"].PutValue("North");
            worksheet.Cells["C5"].PutValue(1200);

            try
            {
                // Bir pivot tablo oluştur
                int pivotIndex = worksheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

                // Alanları bölgelere ekle
                pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
                pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
                pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

                // Pivot tabloyu doldurmak için verileri hesapla
                pivotTable.CalculateData();

                // ValuesField özelliğine erişin (yalnızca okuma)
                PivotField valuesField = pivotTable.ValuesField;

                if (valuesField != null)
                {
                    Console.WriteLine("ValuesField Name: " + valuesField.Name);
                    Console.WriteLine("ValuesField DisplayName: " + valuesField.DisplayName);
                    Console.WriteLine("ValuesField Position: " + valuesField.Position);
                    Console.WriteLine("ValuesField RegionType: " + valuesField.RegionType);
                    Console.WriteLine("ValuesField IsValuesField: " + valuesField.IsValuesField);
                }
                else
                {
                    Console.WriteLine("ValuesField is null - no data fields in the pivot table");
                }

                // Çalışma kitabını kaydedin
                workbook.Save("PivotTableValuesFieldDemo.xlsx");
                Console.WriteLine("PivotTable with ValuesField demonstrated successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


