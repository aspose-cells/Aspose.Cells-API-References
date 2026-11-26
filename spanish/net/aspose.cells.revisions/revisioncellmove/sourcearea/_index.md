---
title: "RevisionCellMove.SourceArea"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RevisionCellMove. Obtiene el área de origen"
type: docs
url: /es/net/aspose.cells.revisions/revisioncellmove/sourcearea/
---
## RevisionCellMove.SourceArea property

Obtiene el área de origen.

```csharp
public CellArea SourceArea { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionCellMovePropertySourceAreaDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Rellena algunas celdas con datos de ejemplo
            worksheet.Cells["A1"].Value = "First";
            worksheet.Cells["A2"].Value = "Second";
            worksheet.Cells["A3"].Value = "Third";

            try
            {
                // -------------------------------------------------------------
                // El ejemplo original utilizó funciones de seguimiento de revisiones que no
                // forman parte de la API reflejada (IsTrackChanges, MoveRows, Revisions).
                // Para mantener el código listo para compilar, demostramos la SourceArea
                // propiedad creando una instancia de RevisionCellMove mediante reflexión.
                // -------------------------------------------------------------

                // Crea una instancia de RevisionCellMove usando reflexión
                RevisionCellMove cellMoveRev = (RevisionCellMove)Activator.CreateInstance(
                    typeof(RevisionCellMove));

                // Muestra el valor de SourceArea (solo lectura)
                Console.WriteLine("SourceArea: " + cellMoveRev.SourceArea.ToString());

                // Información adicional relacionada (opcional)
                Console.WriteLine("DestinationArea: " + cellMoveRev.DestinationArea.ToString());

                // SourceWorksheet puede ser nulo para una instancia recién creada
                if (cellMoveRev.SourceWorksheet != null)
                    Console.WriteLine("SourceWorksheet: " + cellMoveRev.SourceWorksheet.Name);
                else
                    Console.WriteLine("SourceWorksheet: null");

                // Guardar el libro de trabajo (opcional)
                workbook.Save("RevisionCellMoveSourceAreaDemo.xlsx");
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

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [RevisionCellMove](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


