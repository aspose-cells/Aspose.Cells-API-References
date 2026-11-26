---
title: "RevisionCellMove.SourceWorksheet"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RevisionCellMove. Obtiene la hoja de cálculo origen"
type: docs
url: /es/net/aspose.cells.revisions/revisioncellmove/sourceworksheet/
---
## RevisionCellMove.SourceWorksheet property

Obtiene la hoja de cálculo de origen.

```csharp
public Worksheet SourceWorksheet { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellMovePropertySourceWorksheetDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos para que el ejemplo tenga sentido
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Test Value";

            try
            {
                // Crea una instancia de RevisionCellMove usando reflexión
                RevisionCellMove cellMoveRev = (RevisionCellMove)Activator.CreateInstance(
                    typeof(RevisionCellMove));

                // Muestra el valor de la propiedad SourceWorksheet (solo lectura)
                Console.WriteLine("SourceWorksheet: " + cellMoveRev.SourceWorksheet);

                // Contexto adicional (opcional)
                Console.WriteLine("SourceArea: " + cellMoveRev.SourceArea);
                Console.WriteLine("DestinationArea: " + cellMoveRev.DestinationArea);
                Console.WriteLine("Revision Type: " + cellMoveRev.Type);

                // Guardar el libro de trabajo (opcional)
                workbook.Save("SourceWorksheetDemo.xlsx");
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

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [RevisionCellMove](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


