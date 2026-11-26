---
title: "Clase SubtotalSetting"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.SubtotalSetting. Representa la configuración del subtotal"
type: docs
url: /es/net/aspose.cells/subtotalsetting/
---
## SubtotalSetting class

Representa la configuración del subtotal.

```csharp
public class SubtotalSetting
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [GroupBy](../../aspose.cells/subtotalsetting/groupby/) { get; } | El campo por el cual agrupar, como un desplazamiento entero basado en cero |
| [SubtotalFunction](../../aspose.cells/subtotalsetting/subtotalfunction/) { get; } | La función de subtotal. |
| [SummaryBelowData](../../aspose.cells/subtotalsetting/summarybelowdata/) { get; } | Indica si se agrega un resumen debajo de los datos. |
| [TotalList](../../aspose.cells/subtotalsetting/totallist/) { get; } | Una matriz de desplazamientos de campo basados en cero, que indica los campos a los que se añaden los subtotales. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassSubtotalSettingDemo
    {
        public static void Run()
        {
            // Cree un nuevo libro de trabajo para la demostración
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Agregar datos de ejemplo a la hoja de cálculo
                worksheet.Cells["A1"].PutValue("Category");
                worksheet.Cells["B1"].PutValue("Value");
                worksheet.Cells["A2"].PutValue("Group A");
                worksheet.Cells["A3"].PutValue("Group B");
                worksheet.Cells["A4"].PutValue("Group A");
                worksheet.Cells["A5"].PutValue("Group B");
                worksheet.Cells["B2"].PutValue(100);
                worksheet.Cells["B3"].PutValue(200);
                worksheet.Cells["B4"].PutValue(300);
                worksheet.Cells["B5"].PutValue(400);

                // Define el área de celdas para los subtotales
                CellArea area = CellArea.CreateCellArea("A1", "B5");

                // Aplica subtotales a los datos
                worksheet.Cells.Subtotal(
                    area,
                    0, // Group by first column (Category)
                    ConsolidationFunction.Sum,
                    new int[] { 1 }, // Subtotal on second column (Value)
                    true,
                    true,
                    true);

                // Recupera el SubtotalSetting de la hoja de cálculo
                SubtotalSetting subtotalSetting = worksheet.Cells.RetrieveSubtotalSetting(area);

                // Muestra las propiedades del SubtotalSetting
                Console.WriteLine("Subtotal Setting Properties:");
                Console.WriteLine($"GroupBy field index: {subtotalSetting.GroupBy}");
                Console.WriteLine($"Subtotal Function: {subtotalSetting.SubtotalFunction}");
                Console.WriteLine($"TotalList contains column index: {subtotalSetting.TotalList[0]}");
                Console.WriteLine($"Summary Below Data: {subtotalSetting.SummaryBelowData}");

                // Guarda el libro de trabajo
                workbook.Save("SubtotalSettingDemo.xlsx");
                Console.WriteLine("SubtotalSetting demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with SubtotalSetting: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


