---
title: "GlobalizationSettings.GetTableRowTypeOfHeaders"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo GlobalizationSettings. Ottiene il nome del tipo di righe della tabella che costituiscono l'intestazione della tabella. Il valore predefinito è Headers, quindi nella formula Headers rappresenta l'intestazione della tabella"
type: docs
url: /it/net/aspose.cells/globalizationsettings/gettablerowtypeofheaders/
---
## GlobalizationSettings.GetTableRowTypeOfHeaders method

Ottiene il nome del tipo di righe della tabella che comprende l'intestazione della tabella. Il valore predefinito è "Headers", quindi nella formula "#Headers" rappresenta l'intestazione della tabella.

```csharp
public virtual string GetTableRowTypeOfHeaders()
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

    public class GlobalizationSettingsMethodGetTableRowTypeOfHeadersDemo
    {
        public class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override string GetTableRowTypeOfHeaders()
            {
                return "MyHeaders";
            }
        }

        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Price";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 2.5;
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B3"].Value = 1.8;

            // Correzione della creazione di ListObject gestendo il valore di ritorno di Add()
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            // Usa la proprietà DisplayName invece di Name
            table.DisplayName = "FruitTable";

            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            try
            {
                worksheet.Cells["A5"].Formula = "=COUNTA(FruitTable[#MyHeaders])";
                workbook.CalculateFormula();
                Console.WriteLine("Method executed successfully. Header count: " + worksheet.Cells["A5"].Value);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTableRowTypeOfHeaders method: {ex.Message}");
            }

            workbook.Save("MethodGetTableRowTypeOfHeadersDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


