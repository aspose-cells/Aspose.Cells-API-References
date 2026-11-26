---
title: "RevisionFormat.Style"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RevisionFormat. Obtiene el estilo aplicado"
type: docs
url: /es/net/aspose.cells.revisions/revisionformat/style/
---
## RevisionFormat.Style property

Obtiene el estilo aplicado.

```csharp
public Style Style { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionFormatPropertyStyleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo (el seguimiento de revisiones está habilitado por defecto cuando se realizan cambios)
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos y formato para crear una revisión
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Original Value");
            
            // Crear un estilo y aplicarlo a la celda
            Style originalStyle = workbook.CreateStyle();
            originalStyle.Font.Name = "Arial";
            originalStyle.Font.Size = 12;
            originalStyle.Font.IsBold = true;
            cell.SetStyle(originalStyle);

            // Acceder a las revisiones a través de RevisionLogs
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
            foreach (RevisionLog revisionLog in revisionLogs)
            {
                RevisionCollection revisions = revisionLog.Revisions;
                foreach (Revision revision in revisions)
                {
                    if (revision is RevisionFormat revisionFormat)
                    {
                        // Mostrar las propiedades de estilo actuales de la revisión
                        Style style = revisionFormat.Style;
                        Console.WriteLine("Revision Style Font: " + style.Font.Name);
                        Console.WriteLine("Revision Style Font Size: " + style.Font.Size);
                        Console.WriteLine("Revision Style Is Bold: " + style.Font.IsBold);

                        // Nota: La propiedad Style es de solo lectura en RevisionFormat, por lo que no podemos modificarla directamente
                        // Para cambiar el formato, necesitaríamos modificar el estilo de la celda directamente
                    }
                }
            }

            // Guardar el libro de trabajo con revisiones
            workbook.Save("RevisionFormatStyleDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Style](../../../aspose.cells/style/)
* class [RevisionFormat](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


