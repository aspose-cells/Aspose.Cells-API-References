---
title: "SettablePivotGlobalizationSettings.SetTextOfSubTotal"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettablePivotGlobalizationSettings. Establece el texto del tipo PivotFieldSubtotalType en la tabla dinámica"
type: docs
url: /es/net/aspose.cells/settablepivotglobalizationsettings/settextofsubtotal/
---
## SettablePivotGlobalizationSettings.SetTextOfSubTotal method

Establece el texto del tipo [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/) en la tabla dinámica.

```csharp
public void SetTextOfSubTotal(PivotFieldSubtotalType subTotalType, string text)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| subTotalType | PivotFieldSubtotalType | El [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/) |
| texto | String | El texto del tipo dado |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfSubTotalWithPivotFieldSubtoStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo (solo para propósitos de demostración)
            Workbook workbook = new Workbook();

            // Instancia de SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Establecer texto personalizado para el subtotal Sum
                settings.SetTextOfSubTotal(PivotFieldSubtotalType.Sum, "Custom Sum Total");

                // Verificar el cambio
                string sumText = settings.GetTextOfSubTotal(PivotFieldSubtotalType.Sum);
                Console.WriteLine($"Sum subtotal text after change: {sumText}");

                // Establecer texto personalizado para el subtotal Average
                settings.SetTextOfSubTotal(PivotFieldSubtotalType.Average, "Custom Average Total");

                // Verificar el cambio
                string avgText = settings.GetTextOfSubTotal(PivotFieldSubtotalType.Average);
                Console.WriteLine($"Average subtotal text after change: {avgText}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfSubTotal: {ex.Message}");
            }

            // Guardar el libro de trabajo (no hay modificaciones de tabla dinámica en esta demostración)
            workbook.Save("SetTextOfSubTotalDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [PivotFieldSubtotalType](../../../aspose.cells.pivot/pivotfieldsubtotaltype/)
* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


