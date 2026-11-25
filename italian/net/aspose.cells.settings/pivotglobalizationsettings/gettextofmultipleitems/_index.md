---
title: "PivotGlobalizationSettings.GetTextOfMultipleItems"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotGlobalizationSettings. Ottiene il testo dell'etichetta Elementi Multipli nella Tabella Pivot"
type: docs
url: /it/net/aspose.cells.settings/pivotglobalizationsettings/gettextofmultipleitems/
---
## PivotGlobalizationSettings.GetTextOfMultipleItems method

Restituisce il testo dell'etichetta "(Multiple Items)" nella PivotTable.

```csharp
public virtual string GetTextOfMultipleItems()
```

### Valore di ritorno

Il testo dell'etichetta "(Multiple Items)"

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfMultipleItemsDemo
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
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B4"].PutValue(3000);

            // Crea tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Crea e utilizza le impostazioni di globalizzazione
            PivotGlobalizationSettings settings = new PivotGlobalizationSettings();
            
            // Dimostrare GetTextOfMultipleItems e altri metodi chiave
            Console.WriteLine("Multiple Items Text: " + settings.GetTextOfMultipleItems());
            Console.WriteLine("Total Text: " + settings.GetTextOfTotal());
            Console.WriteLine("Grand Total Text: " + settings.GetTextOfGrandTotal());

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


