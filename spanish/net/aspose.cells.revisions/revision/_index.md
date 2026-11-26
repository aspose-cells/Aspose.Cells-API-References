---
title: "Clase Revision"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Revisions.Revision class. Representa la revisión"
type: docs
url: /es/net/aspose.cells.revisions/revision/
---
## Revision class

Representa la revisión.

```csharp
public abstract class Revision
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Obtiene el número de esta revisión. |
| virtual [Type](../../aspose.cells.revisions/revision/type/) { get; } | Representa el tipo de revisión. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Obtiene la hoja de cálculo. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionDemo
    {
        public static void Run()
        {
            // Cree un nuevo libro de trabajo para la demostración
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Agregar algunos datos para potencialmente crear revisiones
                worksheet.Cells["A1"].PutValue("Original Value");

                // Guardar el libro de trabajo para establecer una línea base
                workbook.Save("RevisionDemo_Baseline.xlsx");

                // Cargar el libro de trabajo y realizar un cambio
                Workbook modifiedWorkbook = new Workbook("RevisionDemo_Baseline.xlsx");
                modifiedWorkbook.Worksheets[0].Cells["A1"].PutValue("Modified Value");

                // Verificar si hay registros de revisión
                if (modifiedWorkbook.Worksheets.RevisionLogs.Count > 0)
                {
                    RevisionLog log = modifiedWorkbook.Worksheets.RevisionLogs[0];
                    if (log.Revisions.Count > 0)
                    {
                        // Obtener la primera revisión
                        Revision revision = log.Revisions[0];

                        // Mostrar propiedades de solo lectura
                        Console.WriteLine($"Revision ID: {revision.Id}");
                        Console.WriteLine($"Revision Type: {revision.Type}");
                        Console.WriteLine($"Worksheet Name: {revision.Worksheet.Name}");

                        // Guardar el libro de trabajo modificado
                        modifiedWorkbook.Save("RevisionDemo_Modified.xlsx");
                    }
                    else
                    {
                        Console.WriteLine("No revisions found in the log");
                    }
                }
                else
                {
                    Console.WriteLine("No revision logs available");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with Revision: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


