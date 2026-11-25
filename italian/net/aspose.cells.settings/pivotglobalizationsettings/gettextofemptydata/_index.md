---
title: "PivotGlobalizationSettings.GetTextOfEmptyData"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotGlobalizationSettings. Ottiene il testo dell'etichetta vuota nella PivotTable"
type: docs
url: /it/net/aspose.cells.settings/pivotglobalizationsettings/gettextofemptydata/
---
## PivotGlobalizationSettings.GetTextOfEmptyData method

Restituisce il testo dell'etichetta "(blank)" nella PivotTable.

```csharp
public virtual string GetTextOfEmptyData()
```

### Valore di ritorno

Il testo dei dati vuoti

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfEmptyDataDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B4"].PutValue(1500);

            // Crea tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Creare e utilizzare PivotGlobalizationSettings
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();
            
            // Dimostrare il metodo GetTextOfEmptyData
            Console.WriteLine("Empty Data Text: " + globalizationSettings.GetTextOfEmptyData());

            // Salva la cartella di lavoro
            workbook.Save("PivotGlobalizationDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


