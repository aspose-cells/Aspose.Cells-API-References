---
title: "HtmlTableLoadOptionCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlTableLoadOptionCollection Eigenschaft. Gibt das HtmlTableLoadOption-Element am angegebenen Index zurück"
type: docs
url: /de/net/aspose.cells/htmltableloadoptioncollection/item/
---
## HtmlTableLoadOptionCollection indexer

Gibt das [`HtmlTableLoadOption`](../../htmltableloadoption/)-Element am angegebenen Index zurück.

```csharp
public HtmlTableLoadOption this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der nullbasierte Index des Elements. |

### Rückgabewert

Das Element am angegebenen Index.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Erstelle HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Füge eine neue HtmlTableLoadOption per Tabellenindex hinzu
            int index1 = tableLoadOptions.Add(0);

            // Greife über die Item-Eigenschaft auf das HtmlTableLoadOption zu
            HtmlTableLoadOption option = tableLoadOptions[index1];

            // Konfiguriere die Tabellen-Ladeoption
            option.TableToListObject = true;
            option.TargetSheetIndex = 1;

            // Lade HTML-Datei mit den konfigurierten Optionen
            Workbook workbook = new Workbook("input.html", loadOptions);

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [HtmlTableLoadOption](../../htmltableloadoption/)
* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


