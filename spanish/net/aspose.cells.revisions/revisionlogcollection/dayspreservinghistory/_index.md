---
title: "RevisionLogCollection.DaysPreservingHistory"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RevisionLogCollection. Obtiene y establece el número de días que la aplicación de hoja de cálculo mantendrá el historial de cambios para este libro"
type: docs
url: /es/net/aspose.cells.revisions/revisionlogcollection/dayspreservinghistory/
---
## RevisionLogCollection.DaysPreservingHistory property

Obtiene y establece el número de días que la aplicación de hoja de cálculo mantendrá el historial de cambios para este libro.

```csharp
public int DaysPreservingHistory { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RevisionLogCollectionPropertyDaysPreservingHistoryDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Settings.Shared = true;
            workbook.Worksheets[0].Cells["A1"].PutValue("Test Value");
            
            // Establecer la propiedad DaysPreservingHistory
            workbook.Worksheets.RevisionLogs.DaysPreservingHistory = 40;
            
            string outputPath = "output_DaysPreservingHistory.xlsx";
            workbook.Save(outputPath);
            
            // Recargar para verificar la propiedad
            Workbook loadedWorkbook = new Workbook(outputPath);
            Console.WriteLine("DaysPreservingHistory: " + 
                loadedWorkbook.Worksheets.RevisionLogs.DaysPreservingHistory);
        }
    }
}
```

### Ver también

* class [RevisionLogCollection](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


