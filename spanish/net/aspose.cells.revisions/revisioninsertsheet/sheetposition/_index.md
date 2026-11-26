---
title: "RevisionInsertSheet.SheetPosition"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RevisionInsertSheet. Obtiene la posición basada en cero de la nueva hoja en la barra de pestañas de hojas"
type: docs
url: /es/net/aspose.cells.revisions/revisioninsertsheet/sheetposition/
---
## RevisionInsertSheet.SheetPosition property

Obtiene la posición basada en cero de la nueva hoja en la barra de pestañas de hojas.

```csharp
public int SheetPosition { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionInsertSheetPropertySheetPositionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Settings.Shared = true;

            Worksheet insertedSheet = workbook.Worksheets.Insert(0, SheetType.Worksheet);
            insertedSheet.Name = "NewSheet";

            workbook.Save("revisions_sample.xlsx");

            Workbook reopenedWorkbook = new Workbook("revisions_sample.xlsx");
            foreach (RevisionLog log in reopenedWorkbook.Worksheets.RevisionLogs)
            {
                foreach (Revision revision in log.Revisions)
                {
                    if (revision.Type == RevisionType.InsertSheet)
                    {
                        RevisionInsertSheet ris = (RevisionInsertSheet)revision;
                        Console.WriteLine($"Sheet Name: {ris.Name}, Position: {ris.SheetPosition}");
                    }
                }
            }
        }
    }
}
```

### Ver también

* class [RevisionInsertSheet](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


