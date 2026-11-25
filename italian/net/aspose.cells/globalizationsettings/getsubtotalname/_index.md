---
title: "GlobalizationSettings.GetSubTotalName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo GlobalizationSettings. Ottiene il nome del tipo PivotFieldSubtotalType nella PivotTable"
type: docs
url: /it/net/aspose.cells/globalizationsettings/getsubtotalname/
---
## GlobalizationSettings.GetSubTotalName method

Ottiene il nome del tipo [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/) nella PivotTable.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfSubTotal() method instead.")]
public virtual string GetSubTotalName(PivotFieldSubtotalType subTotalType)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| subTotalType | PivotFieldSubtotalType | Il tipo [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/) |

### Valore di ritorno

Il nome del tipo [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/)

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare il metodo PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Questa proprietà sarà rimossa tra 12 mesi a partire da dicembre 2022. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class GlobalizationSettingsMethodGetSubTotalNameWithPivotFieldSubtotalTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            try
            {
                var globalizationSettings = workbook.Settings.GlobalizationSettings;
                PivotFieldSubtotalType subtotalType = PivotFieldSubtotalType.Sum;
                string subTotalName = ((CustomGlobalizationSettings)globalizationSettings).GetSubTotalName(subtotalType);
                
                Console.WriteLine($"Subtotal name for {subtotalType}: {subTotalName}");
                workbook.Worksheets[0].Cells["A1"].PutValue(subTotalName);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetSubTotalName: {ex.Message}");
            }

            workbook.Save("GlobalizationSettingsMethodGetSubTotalNameDemo.xlsx");
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override string GetSubTotalName(PivotFieldSubtotalType subTotalType)
            {
                return $"Custom {subTotalType}";
            }
        }
    }
}
```

### Vedi anche

* enum [PivotFieldSubtotalType](../../../aspose.cells.pivot/pivotfieldsubtotaltype/)
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


