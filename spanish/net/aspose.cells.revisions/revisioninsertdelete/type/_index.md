---
title: "RevisionInsertDelete.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RevisionInsertDelete. Representa el tipo de revisión"
type: docs
url: /es/net/aspose.cells.revisions/revisioninsertdelete/type/
---
## RevisionInsertDelete.Type property

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

    public class RevisionInsertDeletePropertyTypeDemo
    {
        public static void Run()
        {
            // Cree un nuevo workbook y habilite el seguimiento de revisiones
            Workbook workbook = new Workbook();
            workbook.Worksheets.RevisionLogs.DaysPreservingHistory = 30; // Enable revision tracking by setting days

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Inserte una fila para generar un registro de revisión
            worksheet.Cells.InsertRows(0, 1);

            // Obtenga la colección de revisiones (RevisionLogCollection en sí es la colección)
            RevisionLogCollection revisions = workbook.Worksheets.RevisionLogs;

            // Encuentre el RevisionInsertDelete en las revisiones
            foreach (RevisionLog revisionLog in revisions)
            {
                foreach (Revision revision in revisionLog.Revisions)
                {
                    if (revision is RevisionInsertDelete)
                    {
                        RevisionInsertDelete revisionInsertDelete = (RevisionInsertDelete)revision;

                        // Mostrar el valor de la propiedad Type
                        Console.WriteLine("Revision Type: " + revisionInsertDelete.Type);

                        // Demostrar el uso de la propiedad Type
                        if (revisionInsertDelete.Type == RevisionType.InsertDelete)
                        {
                            Console.WriteLine("This revision represents an insert/delete operation");
                            Console.WriteLine("Affected cell area: " + revisionInsertDelete.CellArea);
                            Console.WriteLine("Action type: " + revisionInsertDelete.ActionType);
                        }

                        break;
                    }
                }
            }

            // Guardar el libro de trabajo con revisiones
            workbook.Save("RevisionInsertDeletePropertyTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [RevisionType](../../revisiontype/)
* class [RevisionInsertDelete](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


