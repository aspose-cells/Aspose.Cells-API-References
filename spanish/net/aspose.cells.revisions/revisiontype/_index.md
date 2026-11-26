---
title: "Enumeración RevisionType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Revisions.RevisionType. Representa el tipo de revisión"
type: docs
url: /es/net/aspose.cells.revisions/revisiontype/
---
## RevisionType enumeration

Representa el tipo de revisión.

```csharp
public enum RevisionType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| CustomView | `0` | Vista personalizada. |
| DefinedName | `1` | Nombre definido. |
| ChangeCells | `2` | Cambio de celdas. |
| AutoFormat | `3` | Formato automático. |
| MergeConflict | `4` | Conflicto de fusión. |
| Comment | `5` | Comentario. |
| Format | `6` | Formato. |
| InsertSheet | `7` | Insertar hoja de cálculo. |
| MoveCells | `8` | Mover celdas. |
| Undo | `9` | Deshacer. |
| QueryTable | `10` | Consultar tabla. |
| InsertDelete | `11` | Insertando o eliminando. |
| RenameSheet | `12` | Renombrar hoja de cálculo. |
| Unknown | `13` | Desconocido. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionTypeDemo
    {
        public static void Run()
        {
            // Cree un nuevo libro de trabajo para la demostración
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Demostrar el uso de diferentes valores del enum RevisionType
                RevisionType customViewType = RevisionType.CustomView;
                RevisionType changeCellsType = RevisionType.ChangeCells;
                RevisionType insertSheetType = RevisionType.InsertSheet;

                // Mostrar los valores del enum y sus valores enteros subyacentes
                Console.WriteLine("CustomView type: " + customViewType + " (Value: " + (int)customViewType + ")");
                Console.WriteLine("ChangeCells type: " + changeCellsType + " (Value: " + (int)changeCellsType + ")");
                Console.WriteLine("InsertSheet type: " + insertSheetType + " (Value: " + (int)insertSheetType + ")");

                // Demostrar la verificación de tipos de revisión
                if (workbook.HasRevisions)
                {
                    Console.WriteLine("Workbook contains revisions");
                }
                else
                {
                    Console.WriteLine("Workbook has no revisions");
                }

                // Guarda el libro de trabajo
                workbook.Save("RevisionTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with RevisionType: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


