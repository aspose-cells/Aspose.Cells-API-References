---
title: "PivotShowValuesSetting.BaseFieldIndex"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotShowValuesSetting özelliği. ShowDataAs hesabı kullanıldığında ShowDataAs hesabı için temel alanı temsil eder"
type: docs
url: /tr/net/aspose.cells.pivot/pivotshowvaluessetting/basefieldindex/
---
## PivotShowValuesSetting.BaseFieldIndex property

ShowDataAs hesaplaması kullanıldığında bir ShowDataAs hesaplaması için temel alanı temsil eder.

```csharp
public int BaseFieldIndex { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotShowValuesSettingPropertyBaseFieldIndexDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Özet tablo için örnek veri ekle
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "A";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["A3"].Value = "B";
            worksheet.Cells["B3"].Value = 150;
            worksheet.Cells["A4"].Value = "C";
            worksheet.Cells["B4"].Value = 200;

            try
            {
                // Özet tablo oluştur
                int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

                // Pivot tabloya alan ekle
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

                // Veri alanını ve onun gösterim değerleri ayarını alın
                PivotField dataField = pivotTable.DataFields[0];
                PivotShowValuesSetting showValuesSetting = dataField.ShowValuesSetting;

                // BaseFieldIndex kullanımını göstermek için hesaplama türünü ayarlayın
                showValuesSetting.CalculationType = PivotFieldDataDisplayFormat.PercentageOf;

                // BaseFieldIndex özelliğini ayarlayın ve alın
                showValuesSetting.BaseFieldIndex = 0;
                Console.WriteLine("BaseFieldIndex value: " + showValuesSetting.BaseFieldIndex);

                // Özet tabloyu yenile ve hesapla
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                // Çalışma kitabını kaydedin
                workbook.Save("BaseFieldIndexDemo.xlsx");
                Console.WriteLine("BaseFieldIndex has been demonstrated successfully.");
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

* class [PivotShowValuesSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


