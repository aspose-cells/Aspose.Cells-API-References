---
title: "RevisionCellChange.OldStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RevisionCellChange. Obtiene el estilo antiguo de la celda"
type: docs
url: /es/net/aspose.cells.revisions/revisioncellchange/oldstyle/
---
## RevisionCellChange.OldStyle property

Obtiene el estilo antiguo de la celda.

```csharp
public Style OldStyle { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellChangePropertyOldStyleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo con seguimiento de revisiones
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer estilo inicial para la celda A1
            Cell cell = worksheet.Cells["A1"];
            Style initialStyle = workbook.CreateStyle();
            initialStyle.Font.Name = "Arial";
            initialStyle.Font.Size = 10;
            initialStyle.Font.Color = System.Drawing.Color.Black;
            cell.SetStyle(initialStyle);
            cell.PutValue("Initial Value");

            // Cambiar el estilo de la celda para crear una revisión
            Style newStyle = workbook.CreateStyle();
            newStyle.Font.Name = "Times New Roman";
            newStyle.Font.Size = 12;
            newStyle.Font.Color = System.Drawing.Color.Red;
            newStyle.Font.IsBold = true;
            cell.SetStyle(newStyle);
            cell.PutValue("Modified Value");

            // Accede a los registros de revisiones
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
            foreach (RevisionLog log in revisionLogs)
            {
                foreach (Revision revision in log.Revisions)
                {
                    if (revision is RevisionCellChange cellChange && cellChange.CellName == "A1")
                    {
                        // Mostrar información del cambio de estilo
                        Console.WriteLine("Cell Name: " + cellChange.CellName);
                        Console.WriteLine("Old Style Font: " + cellChange.OldStyle.Font.Name);
                        Console.WriteLine("Old Style Size: " + cellChange.OldStyle.Font.Size);
                        Console.WriteLine("Old Style Color: " + cellChange.OldStyle.Font.Color);
                        Console.WriteLine("New Style Font: " + cellChange.NewStyle.Font.Name);
                        Console.WriteLine("New Style Size: " + cellChange.NewStyle.Font.Size);
                        Console.WriteLine("New Style Color: " + cellChange.NewStyle.Font.Color);

                        // Demostrar el uso de la propiedad OldStyle
                        if (cellChange.OldStyle.Font.Name == "Arial")
                        {
                            Console.WriteLine("\nThe cell originally had Arial font");
                        }
                    }
                }
            }

            // Guardar el libro de trabajo con revisiones
            workbook.Save("RevisionCellChangePropertyOldStyleDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Style](../../../aspose.cells/style/)
* class [RevisionCellChange](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


