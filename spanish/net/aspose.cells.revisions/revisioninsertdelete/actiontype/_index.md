---
title: "RevisionInsertDelete.ActionType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RevisionInsertDelete. Obtiene el tipo de acción de esta revisión"
type: docs
url: /es/net/aspose.cells.revisions/revisioninsertdelete/actiontype/
---
## RevisionInsertDelete.ActionType property

Obtiene el tipo de acción de esta revisión.

```csharp
public RevisionActionType ActionType { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionInsertDeletePropertyActionTypeDemo
    {
        public static void Run()
        {
            // Cree un nuevo workbook y habilite el seguimiento de revisiones
            Workbook workbook = new Workbook();
            workbook.Worksheets.RevisionLogs.DaysPreservingHistory = 30;

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Realice operaciones para generar revisiones de inserción/eliminación
            worksheet.Cells.InsertRows(0, 1);
            worksheet.Cells.DeleteColumn(0);

            try
            {
                // Obtener los registros de revisiones
                RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

                // Itere a través de todos los registros de revisión para encontrar revisiones de inserción/eliminación
                foreach (RevisionLog revisionLog in revisionLogs)
                {
                    foreach (Revision revision in revisionLog.Revisions)
                    {
                        if (revision is RevisionInsertDelete)
                        {
                            RevisionInsertDelete revisionInsertDelete = (RevisionInsertDelete)revision;

                            // Muestre el valor de la propiedad ActionType
                            Console.WriteLine("ActionType: " + revisionInsertDelete.ActionType);

                            // Demostrar diferentes tipos de acción
                            switch (revisionInsertDelete.ActionType)
                            {
                                case RevisionActionType.InsertRow:
                                    Console.WriteLine("This was a row insertion operation");
                                    break;
                                case RevisionActionType.DeleteColumn:
                                    Console.WriteLine("This was a column deletion operation");
                                    break;
                                case RevisionActionType.Add:
                                    Console.WriteLine("This was an add operation");
                                    break;
                                default:
                                    Console.WriteLine("This was another type of insert/delete operation");
                                    break;
                            }

                            // Mostrar información relacionada
                            Console.WriteLine("Affected cell area: " + revisionInsertDelete.CellArea);
                            Console.WriteLine("Revision type: " + revisionInsertDelete.Type);
                        }
                    }
                }

                // Guardar el libro de trabajo con revisiones
                workbook.Save("ActionTypeDemo.xlsx");
                Console.WriteLine("Workbook saved with revision history.");
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

* enum [RevisionActionType](../../revisionactiontype/)
* class [RevisionInsertDelete](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


