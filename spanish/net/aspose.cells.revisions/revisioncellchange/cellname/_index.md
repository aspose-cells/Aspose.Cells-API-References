---
title: "RevisionCellChange.CellName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RevisionCellChange. Obtiene el nombre de la celda"
type: docs
url: /es/net/aspose.cells.revisions/revisioncellchange/cellname/
---
## RevisionCellChange.CellName property

Obtiene el nombre de la celda.

```csharp
public string CellName { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellChangePropertyCellNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos iniciales para crear una revisión
            worksheet.Cells["A1"].PutValue("Original Value");

            // Modifique la celda para crear una revisión
            worksheet.Cells["A1"].PutValue("Modified Value");

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
                            // Mostrar el valor de la propiedad CellName
                            Console.WriteLine("Cell Name: " + cellChange.CellName);
                            Console.WriteLine("Row Index: " + cellChange.Row);
                            Console.WriteLine("Column Index: " + cellChange.Column);

                            // Demostrar el uso de la propiedad CellName
                            if (cellChange.CellName == "A1")
                            {
                                Console.WriteLine("\nThe revision is for cell A1");
                                Console.WriteLine("Old Value: " + cellChange.OldValue);
                                Console.WriteLine("New Value: " + cellChange.NewValue);
                            }
                        }
                    }
                }

                // Guarda el libro de trabajo
                workbook.Save("RevisionCellChangePropertyCellNameDemo.xlsx");
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


