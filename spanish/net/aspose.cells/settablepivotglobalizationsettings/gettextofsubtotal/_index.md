---
title: "SettablePivotGlobalizationSettings.GetTextOfSubTotal"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettablePivotGlobalizationSettings. Obtiene el texto del tipo PivotFieldSubtotalType en la PivotTable"
type: docs
url: /es/net/aspose.cells/settablepivotglobalizationsettings/gettextofsubtotal/
---
## SettablePivotGlobalizationSettings.GetTextOfSubTotal method

Obtiene el texto del tipo [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/) en la PivotTable.

```csharp
public override string GetTextOfSubTotal(PivotFieldSubtotalType subTotalType)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| subTotalType | PivotFieldSubtotalType | El [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/) |

### Valor de retorno

El texto del tipo dado

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfSubTotalWithPivotFieldSubtotalTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una instancia de SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Llame a GetTextOfSubTotal con diferentes valores de PivotFieldSubtotalType
                string sumText = settings.GetTextOfSubTotal(PivotFieldSubtotalType.Sum);
                string avgText = settings.GetTextOfSubTotal(PivotFieldSubtotalType.Average);
                string countText = settings.GetTextOfSubTotal(PivotFieldSubtotalType.Count);

                // Muestra los resultados
                Console.WriteLine($"Sum subtotal text: {sumText}");
                Console.WriteLine($"Average subtotal text: {avgText}");
                Console.WriteLine($"Count subtotal text: {countText}");

                // Establezca texto personalizado para subtotales
                settings.SetTextOfSubTotal(PivotFieldSubtotalType.Sum, "Custom Sum");
                settings.SetTextOfSubTotal(PivotFieldSubtotalType.Average, "Custom Avg");

                // Verificar los cambios
                Console.WriteLine($"Modified Sum text: {settings.GetTextOfSubTotal(PivotFieldSubtotalType.Sum)}");
                Console.WriteLine($"Modified Avg text: {settings.GetTextOfSubTotal(PivotFieldSubtotalType.Average)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTextOfSubTotal method: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("SettablePivotGlobalizationSettingsDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [PivotFieldSubtotalType](../../../aspose.cells.pivot/pivotfieldsubtotaltype/)
* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


