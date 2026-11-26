---
title: "RevisionLog.MetadataTable"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RevisionLog. Obtiene la tabla que contiene metadatos sobre una lista de cambios específicos que se han producido en este workbook"
type: docs
url: /es/net/aspose.cells.revisions/revisionlog/metadatatable/
---
## RevisionLog.MetadataTable property

Obtiene la tabla que contiene metadatos sobre una lista de cambios específicos que se han producido en este libro de trabajo.

```csharp
public RevisionHeader MetadataTable { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionLogPropertyMetadataTableDemo
    {
        public static void Run()
        {
            // Crea un nuevo libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Realiza algunos cambios para crear historial de revisiones
            worksheet.Cells["A1"].PutValue("Original Value");
            workbook.Save("RevisionDemo.xlsx", SaveFormat.Xlsx);
            
            // Modifique la celda para crear una revisión
            worksheet.Cells["A1"].PutValue("Modified Value");
            workbook.Save("RevisionDemo_modified.xlsx", SaveFormat.Xlsx);

            // Reabrir el workbook modificado para acceder a los registros de revisión
            workbook = new Workbook("RevisionDemo_modified.xlsx");
            
            // Acceder a los registros de revisiones
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
            
            if (revisionLogs.Count > 0)
            {
                RevisionLog revisionLog = revisionLogs[0];
                RevisionHeader metadata = revisionLog.MetadataTable;
                
                Console.WriteLine("Revision Metadata:");
                Console.WriteLine("Saved Time: " + metadata.SavedTime);
                Console.WriteLine("Modified By: " + metadata.UserName);
                Console.WriteLine("Number of Revisions: " + revisionLog.Revisions.Count);
            }
            else
            {
                Console.WriteLine("No revision history found");
            }
        }
    }
}
```

### Ver también

* class [RevisionHeader](../../revisionheader/)
* class [RevisionLog](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


