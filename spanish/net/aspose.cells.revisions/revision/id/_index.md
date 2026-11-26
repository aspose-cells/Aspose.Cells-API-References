---
title: "Revision.Id"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Revision. Obtiene el número de esta revisión"
type: docs
url: /es/net/aspose.cells.revisions/revision/id/
---
## Revision.Id property

Obtiene el número de esta revisión.

```csharp
public int Id { get; }
```

### Observaciones

Cero significa que esta revisión no contiene id.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionPropertyIdDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Realiza un cambio para potencialmente crear una revisión
            worksheet.Cells["A1"].Value = "Sample Data";
            
            try
            {
                // Obtén la colección de registros de revisiones
                RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
                
                if (revisionLogs != null && revisionLogs.Count > 0)
                {
                    // Obtén revisiones del primer registro
                    RevisionCollection revisions = revisionLogs[0].Revisions;
                    
                    if (revisions != null && revisions.Count > 0)
                    {
                        // Accede a la primera revisión
                        Revision revision = revisions[0];
                        
                        // Muestra la propiedad Id (solo lectura)
                        Console.WriteLine("Revision Id: " + revision.Id);
                        
                        // Guarda el libro de trabajo
                        workbook.Save("RevisionIdDemo.xlsx");
                    }
                    else
                    {
                        Console.WriteLine("No revisions found in the log");
                    }
                }
                else
                {
                    Console.WriteLine("No revision logs were created");
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

* class [Revision](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


