---
title: "Enum SaveElementType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Saving.SaveElementType enum. Representa qué tipo de elementos deben guardarse."
type: docs
url: /es/net/aspose.cells.saving/saveelementtype/
---
## SaveElementType enumeration

Representa qué tipo de elementos deben guardarse.

```csharp
public enum SaveElementType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| All | `251658239` | Todos los datos. |
| Chart | `256` | Solo gráficos. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Saving;
    using System;

    public class SavingClassSaveElementTypeDemo
    {
        public static void Run()
        {
            // Cree un nuevo libro de trabajo para la demostración
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Agregar algunos datos de muestra para demostrar el guardado.
                worksheet.Cells["A1"].PutValue("Sample Data");
                worksheet.Cells["B1"].PutValue(12345);

                // Crear un gráfico para demostrar el tipo de elemento de guardado de Chart.
                int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10);
                Chart chart = worksheet.Charts[chartIndex];
                chart.NSeries.Add("A1:B1", true);

                // Demostrar el uso de los valores del enum SaveElementType.
                SaveElementType chartType = SaveElementType.Chart;
                SaveElementType allType = SaveElementType.All;

                Console.WriteLine($"Chart SaveElementType value: {chartType}");
                Console.WriteLine($"All SaveElementType value: {allType}");

                // Guardar el libro de trabajo con todos los elementos.
                OoxmlSaveOptions saveOptions = new OoxmlSaveOptions(SaveFormat.Xlsx);
                workbook.Save("SaveElementTypeDemo.xlsx", saveOptions);
                Console.WriteLine("Workbook saved successfully with all elements");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with SaveElementType: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Saving](../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../)


