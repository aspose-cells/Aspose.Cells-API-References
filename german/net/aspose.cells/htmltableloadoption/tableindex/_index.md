---
title: "HtmlTableLoadOption.TableIndex"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlTableLoadOption-Eigenschaft. Index der Tabelle, die aus HTML importiert werden soll, abrufen oder festlegen"
type: docs
url: /de/net/aspose.cells/htmltableloadoption/tableindex/
---
## HtmlTableLoadOption.TableIndex property

Abrufen oder Festlegen des Index der Tabelle, die aus HTML importiert werden soll.

```csharp
public int TableIndex { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionPropertyTableIndexDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Workbook
            Workbook workbook = new Workbook();

            // HTML-Ladeoptionen erstellen
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Konfigurieren Sie die Tabellenladeoption mit TableIndex = 0 (erste Tabelle)
            HtmlTableLoadOption tableLoadOption = new HtmlTableLoadOption
            {
                TableIndex = 0,
                TableToListObject = true
            };

            // Fügen Sie die Tabellenladeoption hinzu
            loadOptions.TableLoadOptions.Add(tableLoadOption);

            // HTML-Datei laden (durch tatsächlichen Pfad ersetzen)
            workbook = new Workbook("input.html", loadOptions);

            // Als Excel-Datei speichern
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [HtmlTableLoadOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


