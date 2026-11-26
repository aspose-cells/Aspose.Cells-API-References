---
title: "RevisionCellChange.NewValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RevisionCellChange. Obtiene el nuevo valor de la celda"
type: docs
url: /es/net/aspose.cells.revisions/revisioncellchange/newvalue/
---
## RevisionCellChange.NewValue property

Obtiene el nuevo valor de la celda.

```csharp
public object NewValue { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellChangePropertyNewValueDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue datos iniciales a la celda A1
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Original Value");

            // Modifique la celda para crear una revisión
            cell.PutValue("Modified Value");

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
                            // Muestre la propiedad NewValue
                            Console.WriteLine("Cell Name: " + cellChange.CellName);
                            Console.WriteLine("Old Value: " + cellChange.OldValue);
                            Console.WriteLine("New Value: " + cellChange.NewValue);

                            // Demuestre el uso de la propiedad NewValue
                            if (cellChange.NewValue != null)
                            {
                                Console.WriteLine("\nThe new value is: " + cellChange.NewValue.ToString());
                            }
                        }
                    }
                }

                // Guardar el libro de trabajo con revisiones
                workbook.Save("RevisionCellChangePropertyNewValueDemo.xlsx");
                Console.WriteLine("\nWorkbook saved with revisions.");
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


