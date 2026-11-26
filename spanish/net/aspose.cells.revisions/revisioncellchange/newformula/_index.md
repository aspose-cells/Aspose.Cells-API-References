---
title: "RevisionCellChange.NewFormula"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RevisionCellChange. Obtiene la fórmula antigua"
type: docs
url: /es/net/aspose.cells.revisions/revisioncellchange/newformula/
---
## RevisionCellChange.NewFormula property

Obtiene la fórmula anterior.

```csharp
public string NewFormula { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellChangePropertyNewFormulaDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo con seguimiento de revisiones
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Establezca la fórmula inicial en la celda A1
            worksheet.Cells["A1"].Formula = "=SUM(B1:B3)";
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // Cambie la fórmula para crear una revisión
            worksheet.Cells["A1"].Formula = "=AVERAGE(B1:B3)";

            // Accede a los registros de revisiones
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
            foreach (RevisionLog log in revisionLogs)
            {
                foreach (Revision revision in log.Revisions)
                {
                    if (revision is RevisionCellChange cellChange && cellChange.CellName == "A1")
                    {
                        // Muestre información del cambio de fórmula
                        Console.WriteLine("Cell Name: " + cellChange.CellName);
                        Console.WriteLine("Old Formula: " + cellChange.OldFormula);
                        Console.WriteLine("New Formula: " + cellChange.NewFormula);
                        Console.WriteLine("Old Value: " + cellChange.OldValue);
                        Console.WriteLine("New Value: " + cellChange.NewValue);

                        // Demuestre el uso de la propiedad NewFormula
                        if (!string.IsNullOrEmpty(cellChange.NewFormula))
                        {
                            Console.WriteLine("\nThe cell's new formula calculates: " + 
                                worksheet.Cells["A1"].StringValue);
                        }
                    }
                }
            }

            // Guardar el libro de trabajo con revisiones
            workbook.Save("RevisionCellChangePropertyNewFormulaDemo.xlsx");
        }
    }
}
```

### Ver también

* class [RevisionCellChange](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


