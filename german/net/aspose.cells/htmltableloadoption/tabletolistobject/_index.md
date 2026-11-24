---
title: "HtmlTableLoadOption.TableToListObject"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlTableLoadOption-Eigenschaft. Gibt an, ob Listobjekte aus der importierten Tabelle generiert werden. Der Standardwert ist false"
type: docs
url: /de/net/aspose.cells/htmltableloadoption/tabletolistobject/
---
## HtmlTableLoadOption.TableToListObject property

Gibt an, ob Listobjekte aus der importierten Tabelle generiert werden. Der Standardwert ist false.

```csharp
public bool TableToListObject { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionPropertyTableToListObjectDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Workbook
            Workbook workbook = new Workbook();

            // HTML-Ladeoptionen erstellen mit aktivierter TableToListObject
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            HtmlTableLoadOption tableLoadOption = new HtmlTableLoadOption
            {
                TableIndex = 0,
                TableToListObject = true
            };
            loadOptions.TableLoadOptions.Add(tableLoadOption);

            // HTML mit den angegebenen Optionen laden
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


