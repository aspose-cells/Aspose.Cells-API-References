---
title: "RevisionCellChange.Column"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RevisionCellChange. Obtiene el índice de columna de la celda"
type: docs
url: /es/net/aspose.cells.revisions/revisioncellchange/column/
---
## RevisionCellChange.Column property

Obtiene el índice de columna de la celda.

```csharp
public int Column { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellChangePropertyColumnDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo con seguimiento de revisiones
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Modificar la celda B2 para generar una revisión
            Cell cell = worksheet.Cells["B2"];
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
                        // Mostrar información de la columna de la revisión
                        Console.WriteLine("Cell Name: " + cellChange.CellName);
                        Console.WriteLine("Column Index: " + cellChange.Column);
                        Console.WriteLine("Row Index: " + cellChange.Row);

                        // Demostrar el uso de la propiedad Column
                        if (cellChange.Column == 1) // Column B is index 1
                        {
                            Console.WriteLine("\nThis revision affects column B");
                            Console.WriteLine("Old Value: " + cellChange.OldValue);
                            Console.WriteLine("New Value: " + cellChange.NewValue);
                        }
                    }
                }
            }

            // Guardar el libro de trabajo con revisiones
            workbook.Save("RevisionCellChangePropertyColumnDemo.xlsx");
        }
    }
}
```

### Ver también

* class [RevisionCellChange](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


