---
title: "GlobalizationSettings.GetDataFieldHeaderNameOfPivotTable"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GlobalizationSettings yöntemi. PivotTable'daki değer alanı başlık adını alır."
type: docs
url: /tr/net/aspose.cells/globalizationsettings/getdatafieldheadernameofpivottable/
---
## GlobalizationSettings.GetDataFieldHeaderNameOfPivotTable method

PivotTable'daki değer alanı başlık adını alır.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfDataFieldHeader() method instead.")]
public virtual string GetDataFieldHeaderNameOfPivotTable()
```

### Dönüş Değeri

Veri alanı başlık adının adı

### Açıklamalar

NOT: Bu üye artık kullanılmamaktadır. Bunun yerine lütfen PivotGlobalizationSettings.GetColumnLabelsOfPivotTable() metodunu kullanın. Bu özellik, Aralık 2022'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class GlobalizationSettingsMethodGetDataFieldHeaderNameOfPivotTableDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasına erişin
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // PivotTable için örnek veri ekle
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["B1"].Value = "Value";
            worksheet.Cells["A2"].Value = "A";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["A3"].Value = "B";
            worksheet.Cells["B3"].Value = 200;

            // Özel küreselleştirme ayarlarını ayarla
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            try
            {
                // PivotTable oluştur ve alanları yapılandır
                int pivotIndex = worksheet.PivotTables.Add("PivotTable", "A1:B3", "D1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category as row
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);  // Value as data

                // Yerelleştirme değişikliklerini uygulamak için PivotTable'ı yenile
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                Console.WriteLine("PivotTable created with custom data field header name.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // Değiştirilmiş çalışma kitabını kaydet
            workbook.Save("GlobalizationSettingsMethodDemo.xlsx");
        }
    }

    // Özel GlobalizationSettings uygulaması
    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetDataFieldHeaderNameOfPivotTable()
        {
            return "Custom Values";
        }
    }
}
```

### Ayrıca Bakınız

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


