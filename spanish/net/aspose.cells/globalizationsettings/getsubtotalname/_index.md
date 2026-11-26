---
title: "GlobalizationSettings.GetSubTotalName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método GlobalizationSettings. Obtiene el nombre del tipo PivotFieldSubtotalType en la tabla dinámica"
type: docs
url: /es/net/aspose.cells/globalizationsettings/getsubtotalname/
---
## GlobalizationSettings.GetSubTotalName method

Obtiene el nombre del tipo [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/) en la tabla dinámica.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfSubTotal() method instead.")]
public virtual string GetSubTotalName(PivotFieldSubtotalType subTotalType)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| subTotalType | PivotFieldSubtotalType | El tipo [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/) |

### Valor de retorno

El nombre del tipo [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/)

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice el método PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Esta propiedad será eliminada 12 meses después desde diciembre de 2022. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

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

### Ver también

* enum [PivotFieldSubtotalType](../../../aspose.cells.pivot/pivotfieldsubtotaltype/)
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


