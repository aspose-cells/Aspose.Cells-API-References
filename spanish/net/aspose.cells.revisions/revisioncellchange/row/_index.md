---
title: "RevisionCellChange.Row"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RevisionCellChange. Obtiene el índice de fila de la celda"
type: docs
url: /es/net/aspose.cells.revisions/revisioncellchange/row/
---
## RevisionCellChange.Row property

Obtiene el índice de fila de la celda.

```csharp
public int Row { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellChangePropertyRowDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos iniciales para crear una revisión
            worksheet.Cells["B5"].PutValue("Original Value");

            // Modifique la celda para crear una revisión
            worksheet.Cells["B5"].PutValue("Modified Value");

            try
            {
                // Accede a los registros de revisiones
                RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
                foreach (RevisionLog log in revisionLogs)
                {
                    foreach (Revision revision in log.Revisions)
                    {
                        if (revision is RevisionCellChange cellChange)
                        {
                            // Muestra el valor de la propiedad Row
                            Console.WriteLine("Cell Name: " + cellChange.CellName);
                            Console.WriteLine("Row Index: " + cellChange.Row);
                            Console.WriteLine("Column Index: " + cellChange.Column);
                            Console.WriteLine("Old Value: " + cellChange.OldValue);
                            Console.WriteLine("New Value: " + cellChange.NewValue);

                            // Demostrar el uso de la propiedad Row
                            if (cellChange.Row >= 0)
                            {
                                Console.WriteLine("\nThe revision occurred in row " +
                                    (cellChange.Row + 1) + " (1-based index)");
                            }
                        }
                    }
                }

                // Guarda el libro de trabajo
                workbook.Save("RevisionCellChangePropertyRowDemo.xlsx");
                Console.WriteLine("Demo completed successfully.");
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

* class [RevisionCellChange](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


