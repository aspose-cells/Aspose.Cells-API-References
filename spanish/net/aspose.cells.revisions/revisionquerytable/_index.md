---
title: "Clase RevisionQueryTable"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Revisions.RevisionQueryTable. Representa una revisión de un cambio en el campo de una tabla de consulta"
type: docs
url: /es/net/aspose.cells.revisions/revisionquerytable/
---
## RevisionQueryTable class

Representa una revisión de un cambio en el campo de una tabla de consulta.

```csharp
public class RevisionQueryTable : Revision
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [CellArea](../../aspose.cells.revisions/revisionquerytable/cellarea/) { get; } | Obtiene la ubicación de la tabla de consulta afectada. |
| [FieldId](../../aspose.cells.revisions/revisionquerytable/fieldid/) { get; } | Obtiene el ID del campo específico de la tabla de consulta que fue eliminado. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Obtiene el número de esta revisión.(Heredado de [`Revision`](../revision/).) |
| override [Type](../../aspose.cells.revisions/revisionquerytable/type/) { get; } | Representa el tipo de la revisión. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Obtiene la hoja de cálculo. (Heradado de [`Revision`](../revision/).) |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionQueryTableDemo
    {
        public static void Run()
        {
            // Cree un nuevo libro de trabajo para la demostración
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Agrega datos de muestra para crear un contexto para la tabla de consulta
                worksheet.Cells["A1"].Value = "Product";
                worksheet.Cells["B1"].Value = "Price";
                worksheet.Cells["A2"].Value = "Apple";
                worksheet.Cells["B2"].Value = 1.20;

                // Nota: las instancias de RevisionQueryTable se obtienen típicamente de las revisiones del libro de trabajo
                // Esta es una demostración conceptual ya que no podemos instanciar directamente RevisionQueryTable

                // En un escenario real, accederías a las revisiones de esta manera:
                // RevisionCollection revisions = workbook.Worksheets.Revisions;
                // foreach (Revision revision in revisions)
                // {
                //     if (revision is RevisionQueryTable queryTableRevision)
                //     {
                //         // Acceder a las propiedades
                //     }
                // }

                // Para demostración, mostraremos cómo trabajar con las propiedades de RevisionQueryTable
                // si tuviéramos una instancia
                Console.WriteLine("RevisionQueryTable properties demonstration:");
                Console.WriteLine("Type property would return: " + RevisionType.QueryTable);
                Console.WriteLine("FieldId property would return an integer ID of the affected field");
                Console.WriteLine("CellArea property would return the location of the query table");

                // Guarda el libro de trabajo
                workbook.Save("RevisionQueryTableDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with RevisionQueryTable: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


