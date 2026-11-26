---
title: "Enumeración RevisionActionType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Revisions.RevisionActionType enum. Representa el tipo de acción de revisión"
type: docs
url: /es/net/aspose.cells.revisions/revisionactiontype/
---
## RevisionActionType enumeration

Representa el tipo de acción de revisión.

```csharp
public enum RevisionActionType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Add | `0` | Agregar revisión. |
| Delete | `1` | Eliminar revisión. |
| DeleteColumn | `2` | Revisión de eliminación de columna. |
| DeleteRow | `3` | Revisión de eliminación de fila. |
| InsertColumn | `4` | Revisión de inserción de columna. |
| InsertRow | `5` | Revisión de inserción de fila. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionActionTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo con seguimiento de revisiones
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Realizar varias operaciones que generan diferentes tipos de revisión
            worksheet.Cells["A1"].PutValue("Initial Value");
            worksheet.Cells.InsertRow(0);
            worksheet.Cells.DeleteRow(1);
            worksheet.Cells.InsertColumn(0);
            worksheet.Cells.DeleteColumn(1);

            // Verificar si el libro de trabajo tiene revisiones
            if (workbook.HasRevisions)
            {
                // Nota: La API original no proporciona acceso directo a la colección de revisiones
                // Así que solo demostraremos la enumeración RevisionActionType como se solicitó
                Console.WriteLine("Workbook contains revisions (but API doesn't provide access)");
            }

            // Demostrar el uso de los valores de la enumeración RevisionActionType
            Console.WriteLine("Available revision action types:");
            foreach (RevisionActionType actionType in Enum.GetValues(typeof(RevisionActionType)))
            {
                Console.WriteLine($"{actionType} = {(int)actionType}");
            }

            // Guarda el libro de trabajo
            workbook.Save("RevisionActionTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


