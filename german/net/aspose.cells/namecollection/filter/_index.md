---
title: "NameCollection.Filter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "NameCollection-Methode. Gibt alle definierten Namen nach Geltungsbereich zurück"
type: docs
url: /de/net/aspose.cells/namecollection/filter/
---
## NameCollection.Filter method

Ruft alle definierten Namen nach Geltungsbereich ab.

```csharp
public Name[] Filter(NameScopeType type, int sheetIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Typ | NameScopeType | Der Geltungsbereichstyp. |
| sheetIndex | Int32 | Der Blattindex. Wirkt nur, wenn der Geltungsbereichstyp Worksheet ist |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionMethodFilterWithNameScopeTypeInt32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Füge einige Namen zur Arbeitsmappe und zu den Arbeitsblättern hinzu
            workbook.Worksheets.Names.Add("GlobalName");
            Worksheet worksheet1 = workbook.Worksheets[0];
            workbook.Worksheets.Names.Add("Sheet1Name");
            Worksheet worksheet2 = workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Names.Add("Sheet2Name");

            // Filtere Namen nach Geltungsbereichstyp und Blattindex
            Name[] workbookScopeNames = workbook.Worksheets.Names.Filter(NameScopeType.Workbook, -1);
            Name[] worksheetScopeNames = workbook.Worksheets.Names.Filter(NameScopeType.Worksheet, -1);
            Name[] sheet1Names = workbook.Worksheets.Names.Filter(NameScopeType.Worksheet, 0);

            // Ergebnisse ausgeben
            Console.WriteLine($"Workbook-scoped names count: {workbookScopeNames.Length}");
            Console.WriteLine($"Worksheet-scoped names count: {worksheetScopeNames.Length}");
            Console.WriteLine($"Sheet1 names count: {sheet1Names.Length}");
        }
    }
}
```

### Siehe auch

* class [Name](../../name/)
* enum [NameScopeType](../../namescopetype/)
* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


