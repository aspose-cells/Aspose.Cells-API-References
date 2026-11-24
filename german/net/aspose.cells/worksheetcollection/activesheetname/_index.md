---
title: "WorksheetCollection.ActiveSheetName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorksheetCollection-Eigenschaft. Gibt den Namen des aktiven Arbeitsblatts an, wenn die Tabelle geöffnet wird"
type: docs
url: /de/net/aspose.cells/worksheetcollection/activesheetname/
---
## WorksheetCollection.ActiveSheetName property

Stellt den Namen des aktiven Arbeitsblatts dar, wenn die Tabelle geöffnet wird.

```csharp
public string ActiveSheetName { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyActiveSheetNameDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Einige Arbeitsblätter hinzufügen
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Setze das aktive Blatt nach Namen
            workbook.Worksheets.ActiveSheetName = "Sheet2";

            // Überprüfen Sie das aktive Blatt
            Console.WriteLine("Active Sheet: " + workbook.Worksheets.ActiveSheetName);

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


