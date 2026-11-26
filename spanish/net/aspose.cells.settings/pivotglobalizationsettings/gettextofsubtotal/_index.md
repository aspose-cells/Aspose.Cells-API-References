---
title: "PivotGlobalizationSettings.GetTextOfSubTotal"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotGlobalizationSettings. Obtiene el texto del tipo PivotFieldSubtotalType en la PivotTable"
type: docs
url: /es/net/aspose.cells.settings/pivotglobalizationsettings/gettextofsubtotal/
---
## PivotGlobalizationSettings.GetTextOfSubTotal method

Obtiene el texto del tipo [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/) en la PivotTable.

```csharp
public virtual string GetTextOfSubTotal(PivotFieldSubtotalType subTotalType)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| subTotalType | PivotFieldSubtotalType | El [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/) |

### Valor de retorno

El texto del tipo dado

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);

            // Crear tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            Aspose.Cells.Pivot.PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, 1);

            // Crear configuraciones de globalización
            Aspose.Cells.Settings.PivotGlobalizationSettings globalizationSettings = new Aspose.Cells.Settings.PivotGlobalizationSettings();

            // Demostrar GetTextOfSubTotal con diferentes tipos de subtotal
            Console.WriteLine("Sum Subtotal: " + globalizationSettings.GetTextOfSubTotal(Aspose.Cells.Pivot.PivotFieldSubtotalType.Sum));
            Console.WriteLine("Count Subtotal: " + globalizationSettings.GetTextOfSubTotal(Aspose.Cells.Pivot.PivotFieldSubtotalType.Count));
            Console.WriteLine("Average Subtotal: " + globalizationSettings.GetTextOfSubTotal(Aspose.Cells.Pivot.PivotFieldSubtotalType.Average));
            Console.WriteLine("Max Subtotal: " + globalizationSettings.GetTextOfSubTotal(Aspose.Cells.Pivot.PivotFieldSubtotalType.Max));
            Console.WriteLine("Min Subtotal: " + globalizationSettings.GetTextOfSubTotal(Aspose.Cells.Pivot.PivotFieldSubtotalType.Min));

            // Guardar el libro de trabajo
            workbook.Save("PivotGlobalizationDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [PivotFieldSubtotalType](../../../aspose.cells.pivot/pivotfieldsubtotaltype/)
* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


