---
title: "SettableGlobalizationSettings.GetTableRowTypeOfTotals"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettableGlobalizationSettings. Ottiene il nome del tipo di righe della tabella che consiste nella riga totale della tabella di riferimento"
type: docs
url: /it/net/aspose.cells/settableglobalizationsettings/gettablerowtypeoftotals/
---
## SettableGlobalizationSettings.GetTableRowTypeOfTotals method

Ottiene il nome del tipo delle righe della tabella che consiste nella riga totale della tabella di riferimento.

```csharp
public override string GetTableRowTypeOfTotals()
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

    public class SettableGlobalizationSettingsMethodGetTableRowTypeOfTotalsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea dati di esempio per la tabella
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(15);
            worksheet.Cells["A4"].PutValue("Total");
            worksheet.Cells["B4"].PutValue("=SUM(B2:B3)");

            // Crea un ListObject (Tabella)
            int index = worksheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject table = worksheet.ListObjects[index];
            table.ShowTotals = true;

            // Crea impostazioni di globalizzazione personalizzate
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            settings.SetTableRowTypeOfTotals("CustomTotals");

            try
            {
                // Ottieni il tipo di riga della tabella per i totali
                string rowType = settings.GetTableRowTypeOfTotals();
                Console.WriteLine($"Table row type for totals: {rowType}");

                // Applica le impostazioni alla cartella di lavoro
                workbook.Settings.GlobalizationSettings = settings;

                // Verifica l'effetto in una formula
                worksheet.Cells["C2"].Formula = "=SUM(#CustomTotals[B])";
                Console.WriteLine("Formula using custom totals reference: " + worksheet.Cells["C2"].Formula);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTableRowTypeOfTotals method: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("MethodGetTableRowTypeOfTotalsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


