---
title: "RevisionCellChange.NewStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RevisionCellChange. Obtiene el estilo nuevo de la celda"
type: docs
url: /es/net/aspose.cells.revisions/revisioncellchange/newstyle/
---
## RevisionCellChange.NewStyle property

Obtiene el nuevo estilo de la celda.

```csharp
public Style NewStyle { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellChangePropertyNewStyleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo con seguimiento de revisiones
            Workbook workbook = new Workbook();
            // No hay un método StartTrackingRevisions directo disponible - las revisiones se rastrean automáticamente
            Worksheet worksheet = workbook.Worksheets[0];

            // Modifique una celda para generar una revisión
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Original Value");
            Style originalStyle = workbook.CreateStyle();
            originalStyle.Font.Name = "Arial";
            originalStyle.Font.Size = 10;
            cell.SetStyle(originalStyle);

            // Cambie la celda para crear una revisión
            cell.PutValue("New Value");
            Style newStyle = workbook.CreateStyle();
            newStyle.Font.Name = "Times New Roman";
            newStyle.Font.Size = 12;
            newStyle.Font.IsBold = true;
            cell.SetStyle(newStyle);

            // No hay un método StopTrackingRevisions directo disponible

            // Acceda al registro de revisiones a través de RevisionLogs en lugar de Revisions
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
            foreach (RevisionLog log in revisionLogs)
            {
                foreach (Revision revision in log.Revisions)
                {
                    if (revision is RevisionCellChange cellChange)
                    {
                        // Muestre información sobre la revisión de cambio de celda
                        Console.WriteLine("Cell Name: " + cellChange.CellName);
                        Console.WriteLine("Old Value: " + cellChange.OldValue);
                        Console.WriteLine("New Value: " + cellChange.NewValue);

                        // Acceda a la propiedad NewStyle
                        Style revisionNewStyle = cellChange.NewStyle;
                        Console.WriteLine("\nNew Style Properties:");
                        Console.WriteLine("Font Name: " + revisionNewStyle.Font.Name);
                        Console.WriteLine("Font Size: " + revisionNewStyle.Font.Size);
                        Console.WriteLine("Is Bold: " + revisionNewStyle.Font.IsBold);
                    }
                }
            }

            // Guardar el libro de trabajo con revisiones
            workbook.Save("RevisionCellChangePropertyNewStyleDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Style](../../../aspose.cells/style/)
* class [RevisionCellChange](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


