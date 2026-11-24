---
title: "Klasse HtmlTableLoadOption"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.HtmlTableLoadOption Klasse. Stellt die Option beim Importieren einer Tabelle aus HTML dar."
type: docs
url: /de/net/aspose.cells/htmltableloadoption/
---
## HtmlTableLoadOption class

Stellt die Option beim Importieren einer Tabelle aus HTML dar.

```csharp
public class HtmlTableLoadOption
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [HtmlTableLoadOption](htmltableloadoption/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Id](../../aspose.cells/htmltableloadoption/id/) { get; set; } | Abrufen oder Festlegen der ID der Tabelle, die aus HTML importiert werden soll. |
| [Name](../../aspose.cells/htmltableloadoption/name/) { get; set; } | (**Veraltet.**) Abrufen oder Festlegen des Namens der Tabelle, die aus HTML importiert werden soll. |
| [OriginalSheetIndex](../../aspose.cells/htmltableloadoption/originalsheetindex/) { get; set; } | Abrufen oder Festlegen des ursprünglichen Index des Arbeitsblatts im HTML. |
| [TableIndex](../../aspose.cells/htmltableloadoption/tableindex/) { get; set; } | Abrufen oder Festlegen des Index der Tabelle, die aus HTML importiert werden soll. |
| [TableToListObject](../../aspose.cells/htmltableloadoption/tabletolistobject/) { get; set; } | Gibt an, ob Listobjekte aus der importierten Tabelle generiert werden. Der Standardwert ist false. |
| [TargetSheetIndex](../../aspose.cells/htmltableloadoption/targetsheetindex/) { get; set; } | Abrufen oder Festlegen des Zielindex des Arbeitsblatts, in dem die Tabelle platziert werden soll. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlTableLoadOptionDemo
    {
        public static void HtmlTableLoadOptionExample()
        {
            // Erstelle ein neues Workbook
            Workbook workbook = new Workbook();

            // Erstelle eine Instanz von HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Erstelle eine Instanz von HtmlTableLoadOption
            HtmlTableLoadOption tableLoadOption = new HtmlTableLoadOption
            {
                TableIndex = 0,
                Id = "table1",
                Name = "SampleTable",
                OriginalSheetIndex = 0,
                TargetSheetIndex = 0,
                TableToListObject = true
            };

            // Füge die HtmlTableLoadOption zu den HtmlLoadOptions hinzu
            loadOptions.TableLoadOptions.Add(tableLoadOption);

            // Lade die HTML-Datei in das Workbook mit den angegebenen Ladeoptionen
            workbook = new Workbook("HtmlTableLoadOptionExample_original.html", loadOptions);

            // Speichere die Arbeitsmappe in einer Excel‑Datei
            workbook.Save("HtmlTableLoadOptionExample.xlsx");

            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


