---
title: "PivotGlobalizationSettings.GetTextOfTotal"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotGlobalizationSettings. Restituisce il testo dell'etichetta Total nella PivotTable. È necessario sovrascrivere questo metodo quando la PivotTable contiene due o più PivotFields nell'area dati"
type: docs
url: /it/net/aspose.cells.settings/pivotglobalizationsettings/gettextoftotal/
---
## PivotGlobalizationSettings.GetTextOfTotal method

Restituisce il testo dell'etichetta "Total" nella PivotTable. È necessario sovrascrivere questo metodo quando la PivotTable contiene due o più PivotFields nell'area dati.

```csharp
public virtual string GetTextOfTotal()
```

### Valore di ritorno

Il testo dell'etichetta "Totale"

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfTotalDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);

            // Crea tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Crea e utilizza le impostazioni di globalizzazione
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();
            
            // Dimostra il metodo GetTextOfTotal
            Console.WriteLine("Total label text: " + globalizationSettings.GetTextOfTotal());

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


