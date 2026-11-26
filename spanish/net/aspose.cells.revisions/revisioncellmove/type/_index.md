---
title: "RevisionCellMove.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RevisionCellMove. Representa el tipo de revisión"
type: docs
url: /es/net/aspose.cells.revisions/revisioncellmove/type/
---
## RevisionCellMove.Type property

Representa el tipo de revisión.

```csharp
public override RevisionType Type { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellMovePropertyTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Test Value";

            try
            {
                // Crea una instancia de RevisionCellMove usando reflexión
                RevisionCellMove cellMoveRev = (RevisionCellMove)Activator.CreateInstance(
                    typeof(RevisionCellMove));

                // Mostrar el valor de la propiedad Type (solo lectura)
                Console.WriteLine("Revision Type: " + cellMoveRev.Type);

                // Muestra contexto adicional (opcional)
                Console.WriteLine("Source Area: " + cellMoveRev.SourceArea);
                Console.WriteLine("Destination Area: " + cellMoveRev.DestinationArea);

                // Guardar el libro de trabajo (opcional)
                workbook.Save("RevisionCellMoveTypeDemo.xlsx");
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

* enum [RevisionType](../../revisiontype/)
* class [RevisionCellMove](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


