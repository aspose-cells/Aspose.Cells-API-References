---
title: "WorksheetCollection.GetSheetByCodeName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorksheetCollection-Methode. Gibt das Arbeitsblatt anhand des Codenamens zurück"
type: docs
url: /de/net/aspose.cells/worksheetcollection/getsheetbycodename/
---
## WorksheetCollection.GetSheetByCodeName method

Ruft das Arbeitsblatt über den Codenamen ab.

```csharp
public Worksheet GetSheetByCodeName(string codeName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| codeName | String | Arbeitsblatt-Codename. |

### Rückgabewert

Das Element mit dem angegebenen Codenamen.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodGetSheetByCodeNameWithStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Arbeitsblätter hinzufügen und deren Codenamen festlegen
            Worksheet sheet1 = workbook.Worksheets.Add("Sheet1");
            sheet1.CodeName = "MainSheet";
            
            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
            sheet2.CodeName = "DataSheet";

            // Arbeitsblatt nach Codename abrufen
            Worksheet mainSheet = workbook.Worksheets.GetSheetByCodeName("MainSheet");
            Worksheet dataSheet = workbook.Worksheets.GetSheetByCodeName("DataSheet");

            // Demonstrieren Sie die Verwendung, indem Sie in Zellen schreiben
            mainSheet.Cells["A1"].PutValue("This is Main Sheet");
            dataSheet.Cells["A1"].PutValue("This is Data Sheet");

            // Speichere die Arbeitsmappe
            workbook.Save("GetSheetByCodeNameDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


