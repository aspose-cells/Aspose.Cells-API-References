---
title: "HtmlTableLoadOption.Id"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlTableLoadOption-Eigenschaft. ID der Tabelle, die aus HTML importiert werden soll, abrufen oder festlegen"
type: docs
url: /de/net/aspose.cells/htmltableloadoption/id/
---
## HtmlTableLoadOption.Id property

Abrufen oder Festlegen der ID der Tabelle, die aus HTML importiert werden soll.

```csharp
public string Id { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionPropertyIdDemo
    {
        public static void Run()
        {
            // HTML-Ladeoptionen erstellen
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            
            // Tabellennladeoptionen konfigurieren
            HtmlTableLoadOption tableLoadOption1 = new HtmlTableLoadOption();
            tableLoadOption1.Id = "table1"; // Setting Id property
            tableLoadOption1.TargetSheetIndex = 0;
            
            HtmlTableLoadOption tableLoadOption2 = new HtmlTableLoadOption();
            tableLoadOption2.Id = "table2"; // Setting Id property
            tableLoadOption2.TargetSheetIndex = 0;

            // Tabellennladeoptionen hinzufügen
            loadOptions.TableLoadOptions.Add(tableLoadOption1);
            loadOptions.TableLoadOptions.Add(tableLoadOption2);

            // HTML-Datei mit angegebenen Optionen laden
            Workbook workbook = new Workbook("input.html", loadOptions);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
            
            Console.WriteLine("HTML tables with specified IDs have been loaded to Excel.");
        }
    }
}
```

### Siehe auch

* class [HtmlTableLoadOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


