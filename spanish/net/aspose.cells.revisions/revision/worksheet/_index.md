---
title: "Revision.Worksheet"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Revision. Obtiene la hoja de cálculo"
type: docs
url: /es/net/aspose.cells.revisions/revision/worksheet/
---
## Revision.Worksheet property

Obtiene la hoja de cálculo.

```csharp
public Worksheet Worksheet { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionPropertyWorksheetDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer propiedades de la hoja de cálculo
            worksheet.Name = "Demo Sheet";
            worksheet.IsGridlinesVisible = true;
            worksheet.DisplayZeros = false;
            worksheet.Zoom = 120;
            
            // Agregar algunos datos para demostrar revisiones
            worksheet.Cells["A1"].PutValue("Original Value");
            
            // Proteger la hoja de cálculo para habilitar el seguimiento de cambios
            worksheet.Protect(ProtectionType.All);
            
            // Realizar un cambio que se rastreará como revisión
            worksheet.Cells["A1"].PutValue("Modified Value");
            
            // Guardar el libro de trabajo para rastrear revisiones
            workbook.Save("RevisionDemo.xlsx");
            
            // Cargar el libro de trabajo con revisiones
            Workbook workbookWithRevisions = new Workbook("RevisionDemo.xlsx");
            
            // Acceder a los registros de revisiones
            foreach (RevisionLog log in workbookWithRevisions.Worksheets.RevisionLogs)
            {
                foreach (Revision revision in log.Revisions)
                {
                    // Demostrar el acceso a la propiedad Worksheet desde la revisión
                    Console.WriteLine($"Revision Type: {revision.Type}");
                    Console.WriteLine($"Worksheet Name: {revision.Worksheet.Name}");
                    Console.WriteLine($"Worksheet Index: {revision.Worksheet.Index}");
                    
                    if (revision.Type == RevisionType.ChangeCells)
                    {
                        RevisionCellChange cellChange = (RevisionCellChange)revision;
                        Console.WriteLine($"Cell changed in worksheet '{cellChange.Worksheet.Name}': {cellChange.CellName}");
                    }
                }
            }
        }
    }
}
```

### Ver también

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [Revision](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


