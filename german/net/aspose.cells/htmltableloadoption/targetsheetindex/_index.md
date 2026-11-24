---
title: "HtmlTableLoadOption.TargetSheetIndex"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlTableLoadOption-Eigenschaft. Zielindex des Arbeitsblatts, in dem die Tabelle platziert werden soll, abrufen oder festlegen"
type: docs
url: /de/net/aspose.cells/htmltableloadoption/targetsheetindex/
---
## HtmlTableLoadOption.TargetSheetIndex property

Abrufen oder Festlegen des Zielindex des Arbeitsblatts, in dem die Tabelle platziert werden soll.

```csharp
public int TargetSheetIndex { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionPropertyTargetSheetIndexDemo
    {
        public static void Run()
        {
            // HTML-Ladeoptionen erstellen
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            
            // Tabellennladeoptionen mit TargetSheetIndex konfigurieren
            HtmlTableLoadOption tableLoadOption1 = new HtmlTableLoadOption();
            tableLoadOption1.Id = "table1";
            tableLoadOption1.TargetSheetIndex = 0; // Load to first worksheet
            
            HtmlTableLoadOption tableLoadOption2 = new HtmlTableLoadOption();
            tableLoadOption2.Id = "table2";
            tableLoadOption2.TargetSheetIndex = 1; // Load to second worksheet
            
            // Tabellennladeoptionen hinzufügen
            loadOptions.TableLoadOptions.Add(tableLoadOption1);
            loadOptions.TableLoadOptions.Add(tableLoadOption2);
            
            // HTML-Datei mit Optionen laden
            Workbook workbook = new Workbook("input.html", loadOptions);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
            
            // Überprüfen, ob die Tabellen in die richtigen Blätter geladen wurden
            Console.WriteLine("Table1 loaded to sheet index: " + tableLoadOption1.TargetSheetIndex);
            Console.WriteLine("Table2 loaded to sheet index: " + tableLoadOption2.TargetSheetIndex);
        }
    }
}
```

### Siehe auch

* class [HtmlTableLoadOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


