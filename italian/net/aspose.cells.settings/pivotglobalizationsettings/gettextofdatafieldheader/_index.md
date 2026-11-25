---
title: "PivotGlobalizationSettings.GetTextOfDataFieldHeader"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotGlobalizationSettings. Restituisce il testo dell'intestazione del campo dell'area valori nella PivotTable"
type: docs
url: /it/net/aspose.cells.settings/pivotglobalizationsettings/gettextofdatafieldheader/
---
## PivotGlobalizationSettings.GetTextOfDataFieldHeader method

Restituisce il testo dell'intestazione del campo dell'area valori nella PivotTable.

```csharp
public virtual string GetTextOfDataFieldHeader()
```

### Valore di ritorno

Il testo del nome dell'intestazione del campo dati

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfDataFieldHeaderDemo
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
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);

            // Crea tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Crea le impostazioni di globalizzazione e dimostra GetTextOfDataFieldHeader
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();
            Console.WriteLine("Data Field Header Text: " + globalizationSettings.GetTextOfDataFieldHeader());

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


