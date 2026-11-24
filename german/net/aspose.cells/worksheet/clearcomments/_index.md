---
title: "Worksheet.ClearComments"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Methode. Löscht alle Kommentare im Designer-Tabellenblatt"
type: docs
url: /de/net/aspose.cells/worksheet/clearcomments/
---
## Worksheet.ClearComments method

Löscht alle Kommentare im Designer-Tabellenblatt.

```csharp
public void ClearComments()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodClearCommentsDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispielkommentare zu Zellen hinzufügen mittels Zellreferenzen
            int comment1 = worksheet.Comments.Add("A1");
            worksheet.Comments[comment1].Note = "This is comment 1";
            
            int comment2 = worksheet.Comments.Add("B3");
            worksheet.Comments[comment2].Note = "This is comment 2";
            
            int comment3 = worksheet.Comments.Add("C5");
            worksheet.Comments[comment3].Note = "This is comment 3";

            // Kommentaranzahl vor dem Löschen anzeigen
            Console.WriteLine($"Comments count before ClearComments(): {worksheet.Comments.Count}");

            // Alle Kommentare aus dem Arbeitsblatt entfernen
            worksheet.ClearComments();

            // Kommentaranzahl nach dem Löschen anzeigen
            Console.WriteLine($"Comments count after ClearComments(): {worksheet.Comments.Count}");

            // Speichere die Arbeitsmappe
            workbook.Save("ClearCommentsDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


