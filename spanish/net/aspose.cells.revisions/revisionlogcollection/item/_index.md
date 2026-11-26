---
title: "RevisionLogCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RevisionLogCollection. Obtiene RevisionLog por índice"
type: docs
url: /es/net/aspose.cells.revisions/revisionlogcollection/item/
---
## RevisionLogCollection indexer

Obtiene [`RevisionLog`](../../revisionlog/) por índice.

```csharp
public RevisionLog this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice. |

### Valor de retorno

Devuelve el objeto [`RevisionLog`](../../revisionlog/).

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionLogCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Habilitar libro compartido para soportar revisiones
            workbook.Settings.Shared = true;

            // Accede a la colección de registros de revisión
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

            try
            {
                // Verificar si hay registros de revisión
                if (revisionLogs.Count > 0)
                {
                    // Acceder al primer registro de revisión usando la propiedad Item
                    RevisionLog firstLog = revisionLogs[0];

                    // Mostrar información básica sobre el registro de revisión
                    Console.WriteLine("First revision log accessed via Item property:");
                    Console.WriteLine($"Revision count: {firstLog.Revisions.Count}");
                }
                else
                {
                    Console.WriteLine("No revision logs available in the workbook.");
                }

                // Guarda el libro de trabajo
                workbook.Save("RevisionLogItemDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* class [RevisionLog](../../revisionlog/)
* class [RevisionLogCollection](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


