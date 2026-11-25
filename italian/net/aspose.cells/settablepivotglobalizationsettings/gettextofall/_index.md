---
title: "SettablePivotGlobalizationSettings.GetTextOfAll"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettablePivotGlobalizationSettings. Ottiene il testo dell'etichetta All nella PivotTable"
type: docs
url: /it/net/aspose.cells/settablepivotglobalizationsettings/gettextofall/
---
## SettablePivotGlobalizationSettings.GetTextOfAll method

Restituisce il testo dell'etichetta "(All)" nella PivotTable.

```csharp
public override string GetTextOfAll()
```

### Valore di ritorno

Il testo dell'etichetta "(All)"

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfAllDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea dati di esempio per la tabella pivot
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(15);

            // Crea tabella pivot
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Crea impostazioni di globalizzazione
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();
            settings.SetTextOfAll("(All Items)");

            try
            {
                // Ottieni il testo corrente dell'etichetta "(All)"
                string currentText = settings.GetTextOfAll();
                Console.WriteLine($"Current text of '(All)' label: {currentText}");

                // Aggiorna la tabella pivot con le nuove impostazioni
                pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium2;
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                Console.WriteLine("Method executed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTextOfAll method: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("MethodGetTextOfAllDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


