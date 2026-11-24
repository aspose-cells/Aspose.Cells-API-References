---
title: "HtmlTableLoadOptionCollection.TableToListObject"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlTableLoadOptionCollection Eigenschaft. Gibt an, ob ListObjects aus importierten Tabellen erzeugt werden. Der Standardwert ist false"
type: docs
url: /de/net/aspose.cells/htmltableloadoptioncollection/tabletolistobject/
---
## HtmlTableLoadOptionCollection.TableToListObject property

Gibt an, ob Listenobjekte aus importierten Tabellen generiert werden sollen. Der Standardwert ist false.

```csharp
public bool TableToListObject { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionPropertyTableToListObjectDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Workbook
            Workbook workbook = new Workbook();

            // Erstelle HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Greife auf die HtmlTableLoadOptionCollection-Instanz zu
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Setze die TableToListObject-Eigenschaft, um HTML-Tabellen in ListObjects zu konvertieren
            tableLoadOptions.TableToListObject = true;

            // Füge eine Tabelle hinzu, die nach Index in ein ListObject konvertiert werden soll
            tableLoadOptions.Add(0);

            // Laden Sie eine HTML-Datei in die Arbeitsmappe mit den Ladeoptionen
            workbook = new Workbook("input.html", loadOptions);

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


