---
title: "SettableGlobalizationSettings.GetTableRowTypeOfHeaders"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettableGlobalizationSettings. Ottiene il nome del tipo di righe della tabella che costituiscono l'intestazione della tabella. Il valore predefinito è Headers, quindi nella formula Headers rappresenta l'intestazione della tabella"
type: docs
url: /it/net/aspose.cells/settableglobalizationsettings/gettablerowtypeofheaders/
---
## SettableGlobalizationSettings.GetTableRowTypeOfHeaders method

Ottiene il nome del tipo di righe della tabella che comprende l'intestazione della tabella. Il valore predefinito è "Headers", quindi nella formula "#Headers" rappresenta l'intestazione della tabella.

```csharp
public override string GetTableRowTypeOfHeaders()
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

    public class SettableGlobalizationSettingsMethodGetTableRowTypeOfHeadersDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea impostazioni di globalizzazione personalizzate
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            settings.SetTableRowTypeOfHeaders("CustomHeaders");
            workbook.Settings.GlobalizationSettings = settings;

            // Crea dati di esempio per la tabella
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(15);

            try
            {
                // Ottieni il tipo di riga della tabella per le intestazioni
                string rowType = settings.GetTableRowTypeOfHeaders();
                Console.WriteLine($"Table row type for headers: {rowType}");

                // Crea un ListObject (Tabella)
                ListObject table = worksheet.ListObjects[worksheet.ListObjects.Add("A1", "B3", true)];

                // Usa il riferimento dell'intestazione personalizzata in una formula
                worksheet.Cells["C2"].Formula = "=COUNTA(Table1[#CustomHeaders])";
                Console.WriteLine("Formula using custom headers reference: " + worksheet.Cells["C2"].Formula);

                // Calcola la formula
                workbook.CalculateFormula();
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

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


