---
title: "SettableGlobalizationSettings.SetTableRowTypeOfTotals"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettableGlobalizationSettings. Imposta il nome del tipo delle righe di tabella che costituiscono la riga totale della tabella di riferimento"
type: docs
url: /it/net/aspose.cells/settableglobalizationsettings/settablerowtypeoftotals/
---
## SettableGlobalizationSettings.SetTableRowTypeOfTotals method

Imposta il nome del tipo delle righe della tabella che consiste nella riga totale della tabella di riferimento.

```csharp
public void SetTableRowTypeOfTotals(string name)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | il nome del tipo di righe della tabella |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class SettableGlobalizationSettingsMethodSetTableRowTypeOfTotalsWithStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una tabella
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Price");
            cells["A2"].PutValue("Apple");
            cells["B2"].PutValue(10);
            cells["A3"].PutValue("Orange");
            cells["B3"].PutValue(15);
            cells["A4"].PutValue("Total");
            cells["B4"].PutValue("=SUM(B2:B3)");

            int tableIndex = worksheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.ShowTotals = true;

            // Crea impostazioni di globalizzazione
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // Chiama SetTableRowTypeOfTotals con un nome personalizzato
                settings.SetTableRowTypeOfTotals("CustomTotals");

                // Applica le impostazioni alla cartella di lavoro
                workbook.Settings.GlobalizationSettings = settings;

                Console.WriteLine("SetTableRowTypeOfTotals executed successfully with parameter: CustomTotals");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTableRowTypeOfTotals method: {ex.Message}");
            }

            // Salva la cartella di lavoro
            workbook.Save("SetTableRowTypeOfTotalsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


