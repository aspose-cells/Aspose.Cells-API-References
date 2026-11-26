---
title: "RevisionLog.Revisions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RevisionLog. Obtiene todas las revisiones en este registro"
type: docs
url: /es/net/aspose.cells.revisions/revisionlog/revisions/
---
## RevisionLog.Revisions property

Obtiene todas las revisiones en este registro.

```csharp
public RevisionCollection Revisions { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionLogPropertyRevisionsDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con historial de revisiones
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Realizar algunos cambios para rastrear revisiones
            worksheet.Cells["A1"].PutValue("Initial Value");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].Formula = "=A2*2";
            
            // Guardar con seguimiento de revisiones
            workbook.Save("revision_demo.xlsx", SaveFormat.Xlsx);
            
            // Realizar más cambios para crear revisiones
            worksheet.Cells["A1"].PutValue("Modified Value");
            worksheet.Cells["A2"].PutValue(200);
            
            // Guardar de nuevo para registrar revisiones
            workbook.Save("revision_demo.xlsx", SaveFormat.Xlsx);
            
            // Cargar el libro de trabajo con revisiones
            Workbook workbookWithRevisions = new Workbook("revision_demo.xlsx");
            
            // Acceder a los registros de revisiones
            RevisionLogCollection revisionLogs = workbookWithRevisions.Worksheets.RevisionLogs;
            
            // Procesar cada registro de revisiones
            foreach (RevisionLog log in revisionLogs)
            {
                Console.WriteLine($"Processing revision log with {log.Revisions.Count} revisions");
                
                // Acceder a la colección de revisiones
                RevisionCollection revisions = log.Revisions;
                
                foreach (Revision revision in revisions)
                {
                    Console.WriteLine($"Revision Type: {revision.Type}");
                    
                    if (revision.Type == RevisionType.ChangeCells)
                    {
                        RevisionCellChange cellChange = (RevisionCellChange)revision;
                        Console.WriteLine($"Cell {cellChange.CellName} changed from '{cellChange.OldValue}' to '{cellChange.NewValue}'");
                    }
                }
            }
        }
    }
}
```

### Ver también

* class [RevisionCollection](../../revisioncollection/)
* class [RevisionLog](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


