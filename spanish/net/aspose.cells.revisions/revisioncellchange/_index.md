---
title: "Clase RevisionCellChange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Revisions.RevisionCellChange. Representa la revisión que cambia celdas"
type: docs
url: /es/net/aspose.cells.revisions/revisioncellchange/
---
## RevisionCellChange class

Representa la revisión que cambia celdas.

```csharp
public class RevisionCellChange : Revision
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [CellName](../../aspose.cells.revisions/revisioncellchange/cellname/) { get; } | Obtiene el nombre de la celda. |
| [Column](../../aspose.cells.revisions/revisioncellchange/column/) { get; } | Obtiene el índice de columna de la celda. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Obtiene el número de esta revisión.(Heredado de [`Revision`](../revision/).) |
| [IsNewFormatted](../../aspose.cells.revisions/revisioncellchange/isnewformatted/) { get; } | Indica si esta celda está formateada como nueva. |
| [IsOldFormatted](../../aspose.cells.revisions/revisioncellchange/isoldformatted/) { get; } | Indica si esta celda está formateada como antigua. |
| [NewFormula](../../aspose.cells.revisions/revisioncellchange/newformula/) { get; } | Obtiene la fórmula anterior. |
| [NewStyle](../../aspose.cells.revisions/revisioncellchange/newstyle/) { get; } | Obtiene el nuevo estilo de la celda. |
| [NewValue](../../aspose.cells.revisions/revisioncellchange/newvalue/) { get; } | Obtiene el nuevo valor de la celda. |
| [OldFormula](../../aspose.cells.revisions/revisioncellchange/oldformula/) { get; } | Obtiene la fórmula anterior. |
| [OldStyle](../../aspose.cells.revisions/revisioncellchange/oldstyle/) { get; } | Obtiene el estilo antiguo de la celda. |
| [OldValue](../../aspose.cells.revisions/revisioncellchange/oldvalue/) { get; } | Obtiene el valor antiguo de la celda. |
| [Row](../../aspose.cells.revisions/revisioncellchange/row/) { get; } | Obtiene el índice de fila de la celda. |
| override [Type](../../aspose.cells.revisions/revisioncellchange/type/) { get; } | Representa el tipo de revisión. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Obtiene la hoja de cálculo. (Heradado de [`Revision`](../revision/).) |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionsClassRevisionCellChangeDemo
    {
        public static void Run()
        {
            // Crear el directorio de salida si no existe
            string outputDir = "output/";
            System.IO.Directory.CreateDirectory(outputDir);
            
            string filePath = outputDir + "RevisionsClassRevisionCellChangeDemo_out.xlsx";

            // Crear el libro de trabajo inicial y habilitar el uso compartido
            Workbook workbook = new Workbook();
            workbook.Settings.Shared = true;
            workbook.Save(filePath, SaveFormat.Xlsx);

            // Reabrir el libro de trabajo para realizar cambios rastreados
            Workbook workbook2 = new Workbook(filePath);
            Worksheet sheet = workbook2.Worksheets[0];
            
            // Primera revisión: Establecer valores iniciales
            sheet.Cells["A1"].PutValue("Initial Value");
            sheet.Cells["B2"].PutValue(100);
            workbook2.Save(filePath, SaveFormat.Xlsx);
            
            // Segunda revisión: Modificar valores
            sheet.Cells["A1"].PutValue("Updated Value");
            sheet.Cells["B2"].PutValue(200);
            workbook2.Save(filePath, SaveFormat.Xlsx);

            // Cargar el libro de trabajo para acceder a los registros de revisiones
            Workbook workbook3 = new Workbook(filePath);
            
            // Procesar todos los registros de revisiones
            foreach (RevisionLog log in workbook3.Worksheets.RevisionLogs)
            {
                foreach (Revision rev in log.Revisions)
                {
                    if (rev.Type == RevisionType.ChangeCells)
                    {
                        RevisionCellChange rcc = (RevisionCellChange)rev;
                        Console.WriteLine($"Revision Type: {rev.Type}");
                        Console.WriteLine($"Cell: {rcc.CellName} (Row: {rcc.Row}, Column: {rcc.Column})");
                        Console.WriteLine($"Old Value: {rcc.OldValue ?? "null"}");
                        Console.WriteLine($"New Value: {rcc.NewValue ?? "null"}");
                        Console.WriteLine("------------------------------------");
                    }
                }
            }
        }
    }
}
```

### Ver también

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


