---
title: "GlobalizationSettings.GetTableRowTypeOfTotals"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GlobalizationSettings yöntemi. Referans verilen tablonun toplam satırını içeren tablo satırlarının tip adını alır. Varsayılan değer Totals'tır, bu nedenle formülde Totals, referans verilen tablonun toplam satırını temsil eder."
type: docs
url: /tr/net/aspose.cells/globalizationsettings/gettablerowtypeoftotals/
---
## GlobalizationSettings.GetTableRowTypeOfTotals method

Referans alınan tablonun toplam satırını içeren tablo satırlarının tip adını alır. Varsayılan "Totals" olduğundan, "#Totals" formülünde referans alınan tablonun toplam satırını temsil eder.

```csharp
public virtual string GetTableRowTypeOfTotals()
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

    public class GlobalizationSettingsMethodGetTableRowTypeOfTotalsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            try
            {
                worksheet.Cells["A1"].PutValue("Item");
                worksheet.Cells["B1"].PutValue("Price");
                worksheet.Cells["A2"].PutValue("Book");
                worksheet.Cells["B2"].PutValue(25);
                worksheet.Cells["A3"].PutValue("Pen");
                worksheet.Cells["B3"].PutValue(3);
                worksheet.Cells["A4"].PutValue("Notebook");
                worksheet.Cells["B4"].PutValue(10);

                int tableIndex = worksheet.ListObjects.Add("Table1", "A1:B4", true);
                ListObject table = worksheet.ListObjects[tableIndex];
                table.ShowTotals = true;
                table.ListColumns[1].TotalsCalculation = TotalsCalculation.Sum;

                var settings = (CustomGlobalizationSettings)workbook.Settings.GlobalizationSettings;
                string totalRowType = settings.GetTableRowTypeOfTotals();
                
                Console.WriteLine($"Total row type: {totalRowType}");
                worksheet.Cells["C5"].PutValue($"Total row reference: #{totalRowType}");
                
                Console.WriteLine("Method executed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("MethodGetTableRowTypeOfTotalsDemo.xlsx");
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override string GetTableRowTypeOfTotals()
            {
                return "CustomTotals";
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


