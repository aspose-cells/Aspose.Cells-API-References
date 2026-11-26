---
title: "RevisionCellChange.OldValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RevisionCellChange. Obtiene el valor antiguo de la celda"
type: docs
url: /es/net/aspose.cells.revisions/revisioncellchange/oldvalue/
---
## RevisionCellChange.OldValue property

Obtiene el valor antiguo de la celda.

```csharp
public object OldValue { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellChangePropertyOldValueDemo
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
                            // Mostrar el valor de la propiedad OldValue
                            Console.WriteLine("Cell Name: " + cellChange.CellName);
                            Console.WriteLine("Old Value: " + cellChange.OldValue);
                            Console.WriteLine("New Value: " + cellChange.NewValue);

                            // Demostrar el uso de la propiedad OldValue
                            if (cellChange.OldValue != null)
                            {
                                Console.WriteLine("\nThe cell was previously set to: " + cellChange.OldValue);
                            }
                        }
                    }
                }

                // Guarda el libro de trabajo
                workbook.Save("RevisionCellChangePropertyOldValueDemo.xlsx");
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


