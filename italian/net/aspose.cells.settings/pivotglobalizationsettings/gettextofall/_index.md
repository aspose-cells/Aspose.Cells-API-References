---
title: "PivotGlobalizationSettings.GetTextOfAll"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotGlobalizationSettings. Ottiene il testo dell'etichetta Tutto nella Tabella Pivot"
type: docs
url: /it/net/aspose.cells.settings/pivotglobalizationsettings/gettextofall/
---
## PivotGlobalizationSettings.GetTextOfAll method

Restituisce il testo dell'etichetta "(All)" nella PivotTable.

```csharp
public virtual string GetTextOfAll()
```

### Valore di ritorno

Il testo dell'etichetta "(All)"

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfAllDemo
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
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["B3"].PutValue(2000);

            // Crea tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Crea e utilizza le impostazioni di globalizzazione
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();
            
            // Dimostra il metodo GetTextOfAll
            Console.WriteLine("Text of All: " + globalizationSettings.GetTextOfAll());

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


