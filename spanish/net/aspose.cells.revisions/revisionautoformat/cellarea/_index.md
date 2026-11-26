---
title: "RevisionAutoFormat.CellArea"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RevisionAutoFormat. Obtiene la ubicación donde se aplicó el formato"
type: docs
url: /es/net/aspose.cells.revisions/revisionautoformat/cellarea/
---
## RevisionAutoFormat.CellArea property

Obtiene la ubicación donde se aplicó el formato.

```csharp
public CellArea CellArea { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionAutoFormatPropertyCellAreaDemo
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
                    // Demuestra la propiedad CellArea (solo lectura)
                    CellArea area = revisionFormat.CellArea;
                    Console.WriteLine($"Formatting applied to area: StartRow={area.StartRow}, " +
                                      $"StartColumn={area.StartColumn}, EndRow={area.EndRow}, " +
                                      $"EndColumn={area.EndColumn}");
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

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [RevisionAutoFormat](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


