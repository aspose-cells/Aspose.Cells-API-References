---
title: "GlobalizationSettings.GetSubTotalName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GlobalizationSettings-metod. Hämtar namnet på PivotFieldSubtotalType-typen i pivottabellen"
type: docs
url: /sv/net/aspose.cells/globalizationsettings/getsubtotalname/
---
## GlobalizationSettings.GetSubTotalName method

Hämtar namnet på [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/)-typen i pivottabellen.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfSubTotal() method instead.")]
public virtual string GetSubTotalName(PivotFieldSubtotalType subTotalType)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| subTotalType | PivotFieldSubtotalType | Den [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/)-typen |

### Returvärde

Namnet på [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/)-typen

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället PivotGlobalizationSettings.GetColumnLabelsOfPivotTable()‑metoden. Denna egenskap kommer att tas bort 12 månader senare från december 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

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

### Se även

* enum [PivotFieldSubtotalType](../../../aspose.cells.pivot/pivotfieldsubtotaltype/)
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


