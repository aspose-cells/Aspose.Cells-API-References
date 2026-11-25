---
title: "SettableGlobalizationSettings.GetTableRowTypeOfCurrent"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettableGlobalizationSettings. Ottiene il nome del tipo delle righe della tabella che comprende la riga corrente nella tabella di riferimento"
type: docs
url: /it/net/aspose.cells/settableglobalizationsettings/gettablerowtypeofcurrent/
---
## SettableGlobalizationSettings.GetTableRowTypeOfCurrent method

Ottiene il nome del tipo di righe della tabella che comprende la riga corrente nella tabella di riferimento.

```csharp
public override string GetTableRowTypeOfCurrent()
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

    public class SettableGlobalizationSettingsMethodGetTableRowTypeOfCurrentDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una tabella
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Age");
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(30);
            cells["A3"].PutValue("Alice");
            cells["B3"].PutValue(25);

            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.ShowTotals = true;
            table.ListColumns[1].TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum;

            // Crea impostazioni di globalizzazione personalizzate
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            settings.SetTableRowTypeOfCurrent("CurrentRow");

            // Applica le impostazioni alla cartella di lavoro
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // Ottieni il nome del tipo di riga corrente
                string currentRowType = settings.GetTableRowTypeOfCurrent();
                Console.WriteLine("Current row type name: " + currentRowType);

                // Aggiungi una formula che fa riferimento alla riga corrente
                cells["C2"].Formula = "=SUM(#CurrentRow)";
                Console.WriteLine("Formula set to: " + cells["C2"].Formula);

                // Calcola le formule
                workbook.CalculateFormula();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTableRowTypeOfCurrent method: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("MethodGetTableRowTypeOfCurrentDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


