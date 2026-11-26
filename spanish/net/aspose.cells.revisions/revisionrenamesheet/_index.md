---
title: "Clase RevisionRenameSheet"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Revisions.RevisionRenameSheet. Representa una revisión del renombrado de la hoja"
type: docs
url: /es/net/aspose.cells.revisions/revisionrenamesheet/
---
## RevisionRenameSheet class

Representa una revisión del cambio de nombre de una hoja.

```csharp
public class RevisionRenameSheet : Revision
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Obtiene el número de esta revisión.(Heredado de [`Revision`](../revision/).) |
| [NewName](../../aspose.cells.revisions/revisionrenamesheet/newname/) { get; } | Obtiene el nuevo nombre de la hoja de cálculo. |
| [OldName](../../aspose.cells.revisions/revisionrenamesheet/oldname/) { get; } | Obtiene el nombre antiguo de la hoja de cálculo. |
| override [Type](../../aspose.cells.revisions/revisionrenamesheet/type/) { get; } | Representa el tipo de la revisión. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Obtiene la hoja de cálculo. (Heradado de [`Revision`](../revision/).) |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionRenameSheetDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Almacenar el nombre original y renombrar la hoja
                string originalName = worksheet.Name;
                worksheet.Name = "RenamedSheet";

                // Guardar en un flujo de memoria para generar revisiones
                System.IO.MemoryStream ms = new System.IO.MemoryStream();
                workbook.Save(ms, SaveFormat.Xlsx);

                // Reabrir el libro de trabajo para acceder a los registros de revisiones
                workbook = new Workbook(ms);

                // Verificar los registros de revisiones para la operación de renombrado
                foreach (RevisionLog log in workbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision rv in log.Revisions)
                    {
                        if (rv.Type == RevisionType.RenameSheet)
                        {
                            RevisionRenameSheet renameSheet = (RevisionRenameSheet)rv;
                            Console.WriteLine("Revision Type: " + renameSheet.Type);
                            Console.WriteLine("Old Sheet Name: " + renameSheet.OldName);
                            Console.WriteLine("New Sheet Name: " + renameSheet.NewName);
                        }
                    }
                }

                // Guarda el libro de trabajo
                workbook.Save("RevisionRenameSheetDemo.xlsx");
                Console.WriteLine("RevisionRenameSheet demo completed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in RevisionRenameSheet demo: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


