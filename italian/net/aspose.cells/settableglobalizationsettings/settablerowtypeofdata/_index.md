---
title: "SettableGlobalizationSettings.SetTableRowTypeOfData"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettableGlobalizationSettings. Imposta il nome del tipo delle righe della tabella che costituiscono la regione dati della tabella di riferimento"
type: docs
url: /it/net/aspose.cells/settableglobalizationsettings/settablerowtypeofdata/
---
## SettableGlobalizationSettings.SetTableRowTypeOfData method

Imposta il nome del tipo delle righe della tabella che consiste nella regione dati della tabella di riferimento.

```csharp
public void SetTableRowTypeOfData(string name)
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

    public class SettableGlobalizationSettingsMethodSetTableRowTypeOfDataWithStringDemo
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
            table.ListColumns[1].TotalsCalculation = TotalsCalculation.Sum;

            // Crea impostazioni di globalizzazione
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // Imposta un nome personalizzato per le righe dati nella tabella
                settings.SetTableRowTypeOfData("MyDataRegion");
                
                // Applica le impostazioni alla cartella di lavoro
                workbook.Settings.GlobalizationSettings = settings;

                Console.WriteLine("Table row type of data set to: MyDataRegion");
                Console.WriteLine("In formulas, '#MyDataRegion' will now represent the data region instead of '#Data'");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTableRowTypeOfData method: {ex.Message}");
            }

            // Salva la cartella di lavoro
            workbook.Save("SetTableRowTypeOfDataDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


