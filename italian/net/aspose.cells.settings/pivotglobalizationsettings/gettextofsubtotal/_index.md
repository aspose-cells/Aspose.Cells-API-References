---
title: "PivotGlobalizationSettings.GetTextOfSubTotal"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotGlobalizationSettings. Ottiene il testo del tipo PivotFieldSubtotalType nella PivotTable"
type: docs
url: /it/net/aspose.cells.settings/pivotglobalizationsettings/gettextofsubtotal/
---
## PivotGlobalizationSettings.GetTextOfSubTotal method

Ottiene il testo del tipo [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/) nella PivotTable.

```csharp
public virtual string GetTextOfSubTotal(PivotFieldSubtotalType subTotalType)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| subTotalType | PivotFieldSubtotalType | Il [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/) |

### Valore di ritorno

Il testo del tipo specificato

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfSubTotalWithPivotFieldSubtotalTypeDemo
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
            Aspose.Cells.Pivot.PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, 1);

            // Crea impostazioni di globalizzazione
            Aspose.Cells.Settings.PivotGlobalizationSettings globalizationSettings = new Aspose.Cells.Settings.PivotGlobalizationSettings();

            // Dimostrare GetTextOfSubTotal con diversi tipi di subtotale
            Console.WriteLine("Sum Subtotal: " + globalizationSettings.GetTextOfSubTotal(Aspose.Cells.Pivot.PivotFieldSubtotalType.Sum));
            Console.WriteLine("Count Subtotal: " + globalizationSettings.GetTextOfSubTotal(Aspose.Cells.Pivot.PivotFieldSubtotalType.Count));
            Console.WriteLine("Average Subtotal: " + globalizationSettings.GetTextOfSubTotal(Aspose.Cells.Pivot.PivotFieldSubtotalType.Average));
            Console.WriteLine("Max Subtotal: " + globalizationSettings.GetTextOfSubTotal(Aspose.Cells.Pivot.PivotFieldSubtotalType.Max));
            Console.WriteLine("Min Subtotal: " + globalizationSettings.GetTextOfSubTotal(Aspose.Cells.Pivot.PivotFieldSubtotalType.Min));

            // Salva cartella di lavoro
            workbook.Save("PivotGlobalizationDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [PivotFieldSubtotalType](../../../aspose.cells.pivot/pivotfieldsubtotaltype/)
* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


