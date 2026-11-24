---
title: "WorksheetCollection.Names"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorksheetCollection-Eigenschaft. Gibt die Sammlung aller Name-Objekte im Tabellenblatt zurück"
type: docs
url: /de/net/aspose.cells/worksheetcollection/names/
---
## WorksheetCollection.Names property

Ruft die Sammlung aller Name‑Objekte im Tabellenblatt ab.

```csharp
public NameCollection Names { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyNamesDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Ein Arbeitsblatt mit Sonderzeichen im Namen hinzufügen
            Worksheet worksheet = workbook.Worksheets.Add("My.Test");
            
            // Auf die Names-Sammlung zugreifen
            NameCollection names = workbook.Worksheets.Names;
            
            // Einen neuen benannten Bereich hinzufügen
            int index = names.Add("My.Test!TestName");
            Name namedRange = names[index];
            
            // Setze die Bereichsreferenz und demonstriere die Verwendung
            namedRange.RefersTo = "=My.Test!$A$1:$B$2";
            
            // Gib die Eigenschaften des benannten Bereichs aus
            Console.WriteLine("Name: " + namedRange.Text);
            Console.WriteLine("FullText: " + namedRange.FullText);
            Console.WriteLine("RefersTo: " + namedRange.RefersTo);
        }
    }
}
```

### Siehe auch

* class [NameCollection](../../namecollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


