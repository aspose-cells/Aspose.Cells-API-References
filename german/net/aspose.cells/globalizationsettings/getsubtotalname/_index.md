---
title: "GlobalizationSettings.GetSubTotalName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GlobalizationSettings-Methode. Gibt den Namen des PivotFieldSubtotalType-Typs in der PivotTable zurück."
type: docs
url: /de/net/aspose.cells/globalizationsettings/getsubtotalname/
---
## GlobalizationSettings.GetSubTotalName method

Gibt den Namen des [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/) Typs in der PivotTable zurück.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfSubTotal() method instead.")]
public virtual string GetSubTotalName(PivotFieldSubtotalType subTotalType)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| subTotalType | PivotFieldSubtotalType | Der [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/) Typ |

### Rückgabewert

Der Name des [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/) Typs

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Methode PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Diese Eigenschaft wird 12 Monate nach Dezember 2022 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

### Beispiele

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

### Siehe auch

* enum [PivotFieldSubtotalType](../../../aspose.cells.pivot/pivotfieldsubtotaltype/)
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


