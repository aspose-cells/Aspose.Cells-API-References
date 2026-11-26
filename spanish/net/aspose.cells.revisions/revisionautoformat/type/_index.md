---
title: "RevisionAutoFormat.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RevisionAutoFormat. Obtiene el tipo de la revisión"
type: docs
url: /es/net/aspose.cells.revisions/revisionautoformat/type/
---
## RevisionAutoFormat.Type property

Obtiene el tipo de la revisión.

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

    public class RevisionAutoFormatPropertyTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo con seguimiento de revisiones
            Workbook workbook = new Workbook();

            try
            {
                // Accede a la colección de registros de revisión
                RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
                
                // Encuentra la primera instancia de RevisionAutoFormat
                RevisionAutoFormat revisionFormat = null;
                foreach (RevisionLog revisionLog in revisionLogs)
                {
                    foreach (Revision revision in revisionLog.Revisions)
                    {
                        if (revision is RevisionAutoFormat)
                        {
                            revisionFormat = (RevisionAutoFormat)revision;
                            break;
                        }
                    }
                    if (revisionFormat != null) break;
                }

                if (revisionFormat != null)
                {
                    // Demuestra la propiedad Type (solo lectura)
                    RevisionType type = revisionFormat.Type;
                    Console.WriteLine($"Revision type: {type}");
                    
                    // Muestra el valor del enum para mayor claridad
                    Console.WriteLine($"Revision type value: {(int)type}");
                }
                else
                {
                    Console.WriteLine("No auto-format revisions found in the workbook");
                }
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
* class [RevisionAutoFormat](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


