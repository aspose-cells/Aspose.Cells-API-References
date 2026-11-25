---
title: "SettableGlobalizationSettings.SetTableRowTypeOfCurrent"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettableGlobalizationSettings. Imposta il nome del tipo delle righe di tabella che consiste nella riga corrente nella tabella di riferimento"
type: docs
url: /it/net/aspose.cells/settableglobalizationsettings/settablerowtypeofcurrent/
---
## SettableGlobalizationSettings.SetTableRowTypeOfCurrent method

Imposta il nome del tipo delle righe della tabella che consiste nella riga corrente della tabella di riferimento.

```csharp
public void SetTableRowTypeOfCurrent(string name)
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

    public class SettableGlobalizationSettingsMethodSetTableRowTypeOfCurrentWithStringDemo
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
            cells["B2"].PutValue("2.5");
            cells["A3"].PutValue("Banana");
            cells["B3"].PutValue("1.5");
            
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.ShowTotals = true;
            table.ListColumns[1].TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum;

            // Crea impostazioni di globalizzazione
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            try
            {
                // Imposta un nome personalizzato per il tipo di riga corrente
                settings.SetTableRowTypeOfCurrent("CurrentItem");
                
                // Applica le impostazioni alla cartella di lavoro
                workbook.Settings.GlobalizationSettings = settings;

                // Verifica l'impostazione ottenendo nuovamente il valore
                string currentRowType = settings.GetTableRowTypeOfCurrent();
                Console.WriteLine($"Current row type name set to: {currentRowType}");

                // Salva la cartella di lavoro
                workbook.Save("SetTableRowTypeOfCurrentDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTableRowTypeOfCurrent method: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


