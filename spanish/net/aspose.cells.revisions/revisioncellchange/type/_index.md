---
title: "RevisionCellChange.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RevisionCellChange. Representa el tipo de revisión"
type: docs
url: /es/net/aspose.cells.revisions/revisioncellchange/type/
---
## RevisionCellChange.Type property

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

    public class RevisionCellChangePropertyTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo con seguimiento de revisiones
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Habilitar el seguimiento de cambios modificando una celda - las revisiones se rastrean automáticamente
            // cuando se realizan cambios después de la creación del libro de trabajo
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Initial Value");

            // Cambie la celda para crear una revisión
            cell.PutValue("Modified Value");

            // Accede a los registros de revisiones
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
            foreach (RevisionLog log in revisionLogs)
            {
                foreach (Revision revision in log.Revisions)
                {
                    if (revision is RevisionCellChange cellChange)
                    {
                        // Mostrar información del tipo de la revisión
                        Console.WriteLine("Cell Name: " + cellChange.CellName);
                        Console.WriteLine("Revision Type: " + cellChange.Type);

                        // Demostrar el uso de la propiedad Type
                        if (cellChange.Type == RevisionType.ChangeCells)
                        {
                            Console.WriteLine("\nThis is a cell change revision");
                            Console.WriteLine("Old Value: " + cellChange.OldValue);
                            Console.WriteLine("New Value: " + cellChange.NewValue);
                        }

                        // Comprobar otros tipos de revisión posibles
                        switch (cellChange.Type)
                        {
                            case RevisionType.ChangeCells:
                                Console.WriteLine("Handling cell value change revision");
                                break;
                            case RevisionType.Format:
                                Console.WriteLine("Handling format change revision");
                                break;
                            default:
                                Console.WriteLine("Handling other type of revision");
                                break;
                        }
                    }
                }
            }

            // Guardar el libro de trabajo con revisiones
            workbook.Save("RevisionCellChangePropertyTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [RevisionType](../../revisiontype/)
* class [RevisionCellChange](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


