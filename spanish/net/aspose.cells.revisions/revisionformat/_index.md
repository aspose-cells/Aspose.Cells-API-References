---
title: "Clase RevisionFormat"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Revisions.RevisionFormat clase. Representa un registro de revisión de información sobre un cambio de formato"
type: docs
url: /es/net/aspose.cells.revisions/revisionformat/
---
## RevisionFormat class

Representa un registro de revisión de información sobre un cambio de formato.

```csharp
public class RevisionFormat : Revision
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Areas](../../aspose.cells.revisions/revisionformat/areas/) { get; } | El rango al que se aplicó este formato. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Obtiene el número de esta revisión.(Heredado de [`Revision`](../revision/).) |
| [Style](../../aspose.cells.revisions/revisionformat/style/) { get; } | Obtiene el estilo aplicado. |
| override [Type](../../aspose.cells.revisions/revisionformat/type/) { get; } | Obtiene el tipo de revisión. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Obtiene la hoja de cálculo. (Heradado de [`Revision`](../revision/).) |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionFormatDemo
    {
        public static void Run()
        {
            // Crea un nuevo libro con modo compartido para habilitar el seguimiento de revisiones
            Workbook workbook = new Workbook();
            workbook.Settings.Shared = true;
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Agrega algunos datos y aplica formato para crear una revisión
                Cell cell = worksheet.Cells["A1"];
                cell.PutValue("Sample Data");

                // Aplica un estilo para crear una revisión de formato
                Style style = workbook.CreateStyle();
                style.Font.IsBold = true;
                cell.SetStyle(style);

                // Accede a los registros de revisiones
                foreach (RevisionLog revisionLog in workbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision revision in revisionLog.Revisions)
                    {
                        if (revision is RevisionFormat revisionFormat)
                        {
                            // Muestra las propiedades de la revisión
                            Console.WriteLine("Revision Type: " + revisionFormat.Type);
                            Console.WriteLine("Number of affected areas: " + revisionFormat.Areas.Length);

                            // Mostrar información de estilo
                            Style revisionStyle = revisionFormat.Style;
                            Console.WriteLine("Font Name: " + revisionStyle.Font.Name);
                            Console.WriteLine("Font Size: " + revisionStyle.Font.Size);
                            Console.WriteLine("Is Bold: " + revisionStyle.Font.IsBold);
                        }
                    }
                }

                // Guarda el libro de trabajo
                workbook.Save("RevisionFormatDemo.xlsx");
                Console.WriteLine("RevisionFormat demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with RevisionFormat: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


