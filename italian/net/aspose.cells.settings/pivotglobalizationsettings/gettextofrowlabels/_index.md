---
title: "PivotGlobalizationSettings.GetTextOfRowLabels"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotGlobalizationSettings. Ottiene il testo dell'etichetta Etichette di Riga nella Tabella Pivot"
type: docs
url: /it/net/aspose.cells.settings/pivotglobalizationsettings/gettextofrowlabels/
---
## PivotGlobalizationSettings.GetTextOfRowLabels method

Restituisce il testo dell'etichetta "Row Labels" nella PivotTable.

```csharp
public virtual string GetTextOfRowLabels()
```

### Valore di ritorno

Il testo delle etichette di riga

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfRowLabelsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Fruit");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Vegetable");
            worksheet.Cells["B3"].PutValue(200);

            // Crea tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Crea e utilizza le impostazioni di globalizzazione
            PivotGlobalizationSettings settings = new PivotGlobalizationSettings();
            
            // Dimostra GetTextOfRowLabels
            Console.WriteLine("Row Labels Text: " + settings.GetTextOfRowLabels());

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


