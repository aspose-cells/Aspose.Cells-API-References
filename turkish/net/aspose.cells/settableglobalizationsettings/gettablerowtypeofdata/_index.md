---
title: "SettableGlobalizationSettings.GetTableRowTypeOfData"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SettableGlobalizationSettings yöntemi. Referans alınan tablonun veri bölgesinden oluşan tablo satırlarının tip adını alır. Varsayılan Data'dır, bu nedenle formülde Data tabloyun veri bölgesini temsil eder"
type: docs
url: /tr/net/aspose.cells/settableglobalizationsettings/gettablerowtypeofdata/
---
## SettableGlobalizationSettings.GetTableRowTypeOfData method

Referans verilen tablonun veri bölgesini içeren tablo satırlarının tip adını alır. Varsayılan "Data"dır, bu yüzden formülde "#Data" tabloyun veri bölgesini temsil eder.

```csharp
public override string GetTableRowTypeOfData()
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

    public class SettableGlobalizationSettingsMethodGetTableRowTypeOfDataDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
                settings.SetTableRowTypeOfData("CustomData");
                string rowType = settings.GetTableRowTypeOfData();
                Console.WriteLine($"TableRowTypeOfData: {rowType}");

                workbook.Settings.GlobalizationSettings = settings;

                worksheet.Cells["A1"].PutValue("Product");
                worksheet.Cells["A2"].PutValue("Apple");
                worksheet.Cells["A3"].PutValue("Orange");
                worksheet.Cells["B1"].PutValue("Price");
                worksheet.Cells["B2"].PutValue(5.5);
                worksheet.Cells["B3"].PutValue(3.8);

                int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
                ListObject table = worksheet.ListObjects[tableIndex];
                table.DisplayName = "Inventory"; // Changed from Name to DisplayName
                
                worksheet.Cells["B4"].Formula = "=SUM(Inventory[#CustomData][Price])";
                
                workbook.CalculateFormula();
                Console.WriteLine($"Total price: {worksheet.Cells["B4"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("MethodGetTableRowTypeOfDataDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


