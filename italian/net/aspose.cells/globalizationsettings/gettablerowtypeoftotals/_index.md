---
title: "GlobalizationSettings.GetTableRowTypeOfTotals"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo GlobalizationSettings. Ottiene il nome del tipo di righe della tabella che consiste nella riga totale della tabella di riferimento. Il valore predefinito è Totals, quindi nella formula Totals rappresenta la riga totale della tabella di riferimento"
type: docs
url: /it/net/aspose.cells/globalizationsettings/gettablerowtypeoftotals/
---
## GlobalizationSettings.GetTableRowTypeOfTotals method

Ottiene il nome del tipo di righe della tabella che comprende la riga totale della tabella di riferimento. Il valore predefinito è "Totals", quindi nella formula "#Totals" rappresenta la riga totale della tabella di riferimento.

```csharp
public virtual string GetTableRowTypeOfTotals()
```

### Valore di ritorno

il nome del tipo di righe della tabella

### Esempi

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

### Vedi anche

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


