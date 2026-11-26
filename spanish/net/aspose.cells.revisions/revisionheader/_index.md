---
title: "Clase RevisionHeader"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Revisions.RevisionHeader. Representa una lista de cambios específicos que se han producido en este libro de trabajo"
type: docs
url: /es/net/aspose.cells.revisions/revisionheader/
---
## RevisionHeader class

Representa una lista de cambios específicos que han ocurrido en este libro de trabajo.

```csharp
public class RevisionHeader
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [RevisionHeader](revisionheader/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [SavedTime](../../aspose.cells.revisions/revisionheader/savedtime/) { get; set; } | Obtiene y establece la fecha y hora en que se guardó este conjunto de revisiones. |
| [UserName](../../aspose.cells.revisions/revisionheader/username/) { get; set; } | Obtiene y establece el nombre del usuario que realiza la revisión. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionHeaderDemo
    {
        public static void Run()
        {
            // Cree un nuevo libro de trabajo para la demostración
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Crea una instancia de la clase RevisionHeader
                RevisionHeader revisionHeader = new RevisionHeader();

                // Establece propiedades esenciales
                revisionHeader.SavedTime = DateTime.Now;
                revisionHeader.UserName = "TestUser";

                // Demuestra la funcionalidad básica
                Console.WriteLine($"Revision saved by: {revisionHeader.UserName}");
                Console.WriteLine($"Revision saved at: {revisionHeader.SavedTime}");

                // Guarda el libro de trabajo
                workbook.Save("RevisionHeaderDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with revision header information.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with RevisionHeader: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


