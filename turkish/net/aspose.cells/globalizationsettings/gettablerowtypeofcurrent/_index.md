---
title: "GlobalizationSettings.GetTableRowTypeOfCurrent"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GlobalizationSettings yöntemi. Referans alınan tabloda mevcut satırı içeren tablo satırlarının tip adını alır. Varsayılan değer This Row'dur, bu nedenle formülde This Row referans alınan tabloda mevcut satırı temsil eder."
type: docs
url: /tr/net/aspose.cells/globalizationsettings/gettablerowtypeofcurrent/
---
## GlobalizationSettings.GetTableRowTypeOfCurrent method

Referans alınan tablodaki mevcut satırı içeren tablo satırlarının tip adını alır. Varsayılan "This Row" olduğundan, "#This Row" formülünde referans alınan tablonun mevcut satırını temsil eder.

```csharp
public virtual string GetTableRowTypeOfCurrent()
```

### Dönüş Değeri

tablo satırlarının tip adı

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class GlobalizationSettingsMethodGetTableRowTypeOfCurrentDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Özel küreselleştirme ayarlarını ayarla
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            try
            {
                // Örnek veri ve tablo oluşturun
                worksheet.Cells["A1"].PutValue("Product");
                worksheet.Cells["B1"].PutValue("Price");
                worksheet.Cells["A2"].PutValue("Apple");
                worksheet.Cells["B2"].PutValue(2.5);
                worksheet.Cells["A3"].PutValue("Orange");
                worksheet.Cells["B3"].PutValue(1.8);

                // Tablo oluşturun
                int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
                ListObject table = worksheet.ListObjects[tableIndex];
                table.DisplayName = "PriceTable"; // Fixed property name

                // Mevcut satır referansını kullanarak formül ekleyin
                Cell formulaCell = worksheet.Cells["C2"];
                formulaCell.Formula = "=PriceTable[@Price] * 1.2";

                // GetTableRowTypeOfCurrent etkisini gösterin
                Console.WriteLine("Generated formula: " + formulaCell.Formula);
                Console.WriteLine("Method executed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTableRowTypeOfCurrent method: {ex.Message}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("MethodGetTableRowTypeOfCurrentDemo.xlsx");
        }
    }

    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetTableRowTypeOfCurrent()
        {
            return "CurrentItem"; // Custom current row identifier
        }
    }
}
```

### Ayrıca Bakınız

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


