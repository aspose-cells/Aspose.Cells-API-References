---
title: "HtmlTableLoadOption.Name"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlTableLoadOption-Eigenschaft. Namen der Tabelle, die aus HTML importiert werden soll, abrufen oder festlegen"
type: docs
url: /de/net/aspose.cells/htmltableloadoption/name/
---
## HtmlTableLoadOption.Name property

Namen der Tabelle, die aus HTML importiert werden soll, abrufen oder festlegen

```csharp
[Obsolete("Please use HtmlTableLoadOption.Id instead")]
public string Name { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionPropertyNameDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Workbook
            Workbook workbook = new Workbook();

            // Erstelle HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Auf die HtmlTableLoadOptionCollection zugreifen
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Füge eine neue HtmlTableLoadOption per Tabellenindex hinzu
            int index = tableLoadOptions.Add(0);

            // Auf die HtmlTableLoadOption zugreifen
            HtmlTableLoadOption option = tableLoadOptions[index];

            // Name-Eigenschaft festlegen
            option.Name = "CustomerDataTable";

            // Eine HTML-Datei laden (durch tatsächlichen Dateipfad ersetzen)
            workbook = new Workbook("input.html", loadOptions);

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [HtmlTableLoadOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


