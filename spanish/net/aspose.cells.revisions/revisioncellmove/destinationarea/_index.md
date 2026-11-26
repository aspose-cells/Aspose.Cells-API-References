---
title: "RevisionCellMove.DestinationArea"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RevisionCellMove. Obtiene el área de destino"
type: docs
url: /es/net/aspose.cells.revisions/revisioncellmove/destinationarea/
---
## RevisionCellMove.DestinationArea property

Obtiene el área de destino.

```csharp
public CellArea DestinationArea { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Revisions;

    public class RevisionCellMovePropertyDestinationAreaDemo
    {
        public static void Run()
        {
            // Crea un libro de trabajo para disponer de un entorno válido (opcional para la demostración)
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Demo";

            try
            {
                // Instancia RevisionCellMove mediante reflexión (constructor sin parámetros)
                RevisionCellMove revMove = (RevisionCellMove)Activator.CreateInstance(typeof(RevisionCellMove));

                // Lee y muestra la propiedad DestinationArea (solo lectura)
                CellArea destination = revMove.DestinationArea;
                Console.WriteLine("DestinationArea: " + destination.ToString());

                // Contexto adicional (opcional)
                Console.WriteLine("SourceArea: " + revMove.SourceArea.ToString());
                Console.WriteLine("Revision Type: " + revMove.Type);

                // Guarda el libro de trabajo (opcional)
                workbook.Save("RevisionCellMoveDestinationAreaDemo.xlsx");
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


