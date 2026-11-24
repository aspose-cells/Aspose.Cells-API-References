---
title: "NameCollection.RemoveDuplicateNames"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "NameCollection‑Methode. Entfernt die doppelt definierten Namen"
type: docs
url: /de/net/aspose.cells/namecollection/removeduplicatenames/
---
## NameCollection.RemoveDuplicateNames method

Entfernt die doppelten definierten Namen

```csharp
public void RemoveDuplicateNames()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionMethodRemoveDuplicateNamesDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie einige benannte Bereiche mit doppelten Namen hinzu
            worksheet.Cells["A1"].PutValue("Test Value 1");
            worksheet.Cells["B1"].PutValue("Test Value 2");
            
            // Erstellen Sie doppelte benannte Bereiche mit der korrekten Add‑Methodensignatur
            int index1 = workbook.Worksheets.Names.Add("DuplicateName");
            workbook.Worksheets.Names[index1].RefersTo = "=Sheet1!$A$1";
            
            int index2 = workbook.Worksheets.Names.Add("DuplicateName");
            workbook.Worksheets.Names[index2].RefersTo = "=Sheet1!$B$1";
            
            // Anzahl vor dem Entfernen von Duplikaten anzeigen
            Console.WriteLine($"Named ranges count before removal: {workbook.Worksheets.Names.Count}");
            
            // Doppelte Namen entfernen
            workbook.Worksheets.Names.RemoveDuplicateNames();
            
            // Anzahl nach dem Entfernen von Duplikaten anzeigen
            Console.WriteLine($"Named ranges count after removal: {workbook.Worksheets.Names.Count}");
        }
    }
}
```

### Siehe auch

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


