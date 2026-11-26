---
title: "Worksheet.GetSelectedRanges"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de Worksheet. Obtiene los rangos de celdas seleccionados en la hoja de cálculo del diseñador"
type: docs
url: /es/net/aspose.cells/worksheet/getselectedranges/
---
## Worksheet.GetSelectedRanges method

Obtiene los rangos de celdas seleccionados en la hoja de cálculo del diseñador.

```csharp
[Obsolete("Use Worksheet.GetSelectedAreas() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList GetSelectedRanges()
```

### Valor de retorno

Una ArrayList que contiene los rangos seleccionados.

### Observaciones

NOTA: Este método está ahora obsoleto. En su lugar, utilice el método Worksheet.GetSelectedAreas(). Esta propiedad será eliminada 12 meses después desde marzo de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class WorksheetMethodGetSelectedRangesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B2"].Value = "Test Value";

            try
            {
                // Nota: GetSelectedRanges está marcado como obsoleto en la reflexión
                // Esto demuestra la llamada al método según lo solicitado
                ArrayList selectedRanges = worksheet.GetSelectedRanges();

                // Mostrar el número de rangos seleccionados
                Console.WriteLine($"Number of selected ranges: {selectedRanges.Count}");

                // Mostrar cada rango seleccionado
                foreach (var range in selectedRanges)
                {
                    Console.WriteLine($"Selected range: {range}");
                }

                // Guarda el libro de trabajo
                workbook.Save("GetSelectedRangesDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


