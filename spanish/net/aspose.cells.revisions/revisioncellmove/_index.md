---
title: "Clase RevisionCellMove"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Revisions.RevisionCellMove. Representa un registro de revisión en una celda que se movió"
type: docs
url: /es/net/aspose.cells.revisions/revisioncellmove/
---
## RevisionCellMove class

Representa un registro de revisión de una(s) celda(s) que se movió(ron).

```csharp
public class RevisionCellMove : Revision
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [DestinationArea](../../aspose.cells.revisions/revisioncellmove/destinationarea/) { get; } | Obtiene el área de destino. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Obtiene el número de esta revisión.(Heredado de [`Revision`](../revision/).) |
| [SourceArea](../../aspose.cells.revisions/revisioncellmove/sourcearea/) { get; } | Obtiene el área de origen. |
| [SourceWorksheet](../../aspose.cells.revisions/revisioncellmove/sourceworksheet/) { get; } | Obtiene la hoja de cálculo de origen. |
| override [Type](../../aspose.cells.revisions/revisioncellmove/type/) { get; } | Representa el tipo de revisión. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Obtiene la hoja de cálculo. (Heradado de [`Revision`](../revision/).) |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionCellMoveDemo
    {
        public static void Run()
        {
            // Cree un nuevo libro de trabajo para la demostración
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Crea una instancia de la clase RevisionCellMove usando reflexión
                // ya que el constructor no es accesible directamente
                RevisionCellMove revisionCellMove = (RevisionCellMove)Activator.CreateInstance(
                    typeof(RevisionCellMove));

                // Mostrar las propiedades de solo lectura
                Console.WriteLine("Revision Type: " + revisionCellMove.Type);
                Console.WriteLine("Source Area: " + revisionCellMove.SourceArea);
                Console.WriteLine("Destination Area: " + revisionCellMove.DestinationArea);

                // Verifica si SourceWorksheet está disponible
                if (revisionCellMove.SourceWorksheet != null)
                {
                    Console.WriteLine("Source Worksheet: " + revisionCellMove.SourceWorksheet.Name);
                }
                else
                {
                    Console.WriteLine("Source Worksheet: null");
                }

                // Guarda el libro de trabajo
                workbook.Save("RevisionCellMoveDemo.xlsx");
                Console.WriteLine("RevisionCellMove demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with RevisionCellMove: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


