---
title: "FindOptions.SearchNext"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FindOptions‑Eigenschaft. Suchreihenfolge. True: nächstes suchen. False: vorheriges suchen"
type: docs
url: /de/net/aspose.cells/findoptions/searchnext/
---
## FindOptions.SearchNext property

Suchreihenfolge. True: nächstes suchen. False: vorheriges suchen.

```csharp
[Obsolete("Use FindOptions.SearchBackward property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool SearchNext { get; set; }
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Bitte verwenden Sie stattdessen die FindOptions.SearchBackward‑Eigenschaft. Diese Eigenschaft wird 12 Monate später, seit November 2018, entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FindOptionsPropertySearchNextDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Einige Beispieldaten einfügen
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("apple");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["A5"].PutValue("apple pie");

            // Suchoptionen erstellen
            FindOptions findOptions = new FindOptions();
            findOptions.CaseSensitive = false;
            findOptions.LookAtType = LookAtType.Contains;

            // Demonstriere die SearchNext‑Eigenschaft (veraltet, aber zur Demonstration gezeigt)
            Console.WriteLine("Initial SearchNext value: " + findOptions.SearchNext);
            
            // Vorwärts suchen (Standardverhalten)
            findOptions.SearchNext = true;
            Cell firstForward = worksheet.Cells.Find("apple", null, findOptions);
            Console.WriteLine("First forward search result: " + (firstForward != null ? firstForward.Name + " - " + firstForward.StringValue : "Not found"));

            // Rückwärts suchen
            findOptions.SearchNext = false;
            Cell firstBackward = worksheet.Cells.Find("apple", null, findOptions);
            Console.WriteLine("First backward search result: " + (firstBackward != null ? firstBackward.Name + " - " + firstBackward.StringValue : "Not found"));

            // Speichere die Arbeitsmappe
            workbook.Save("PropertySearchNextDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


