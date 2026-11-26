---
title: "RevisionFormat.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RevisionFormat. Obtiene el tipo de revisión"
type: docs
url: /es/net/aspose.cells.revisions/revisionformat/type/
---
## RevisionFormat.Type property

Obtiene el tipo de revisión.

```csharp
public override RevisionType Type { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionFormatPropertyTypeDemo
    {
        public static void Run()
        {
            // Crea un nuevo libro con modo compartido para habilitar el seguimiento de revisiones
            Workbook workbook = new Workbook();
            workbook.Settings.Shared = true;

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega algunos datos y aplica formato para crear una revisión
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Data");

            // Aplica un estilo para crear una revisión de formato
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            cell.SetStyle(style);

            try
            {
                // Accede a los registros de revisiones
                foreach (RevisionLog revisionLog in workbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision revision in revisionLog.Revisions)
                    {
                        if (revision is RevisionFormat revisionFormat)
                        {
                            // Mostrar el valor de la propiedad Type
                            Console.WriteLine("Revision Type: " + revisionFormat.Type);

                            // Mostrar información adicional sobre la revisión
                            Console.WriteLine("Number of affected areas: " + revisionFormat.Areas.Length);
                        }
                    }
                }

                // Guarda el libro de trabajo
                workbook.Save("RevisionFormatTypeDemo.xlsx");
                Console.WriteLine("Type property has been demonstrated successfully.");
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

* enum [RevisionType](../../revisiontype/)
* class [RevisionFormat](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


