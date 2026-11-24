---
title: "HtmlLoadOptions.TableLoadOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlLoadOptions-Eigenschaft. Gibt die HtmlTableLoadOptionCollection-Instanz zurück"
type: docs
url: /de/net/aspose.cells/htmlloadoptions/tableloadoptions/
---
## HtmlLoadOptions.TableLoadOptions property

Holt die HtmlTableLoadOptionCollection‑Instanz

```csharp
public HtmlTableLoadOptionCollection TableLoadOptions { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyTableLoadOptionsDemo
    {
        public static void Run()
        {
            // HTML-Ladeoptionen erstellen
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            loadOptions.SupportDivTag = true;
            
            // Tabellennladeoptionen nach Index hinzufügen
            loadOptions.TableLoadOptions.Add(1);
            loadOptions.TableLoadOptions.Add(2);
            
            // Tabellennladeoptionen nach ID hinzufügen
            HtmlTableLoadOption tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = "table1";
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            
            tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = "table2";
            loadOptions.TableLoadOptions.Add(tableLoadOption);

            // HTML-Datei mit den Optionen laden
            Workbook workbook = new Workbook("input.html", loadOptions);
            
            // Ausgabe speichern
            workbook.Save("output.xlsx");
            
            // Vorhandene löschen und neue Tabellennladeoptionen hinzufügen
            loadOptions.TableLoadOptions.Clear();
            
            // Tabellennladeoptionen mit Blatt-Index-Zuordnung hinzufügen
            loadOptions.TableLoadOptions.Add(0, 2); // Table index 0 -> Sheet 2
            loadOptions.TableLoadOptions.Add(1, 0); // Table index 1 -> Sheet 0
            
            // Tabellennladeoptionen mit ID- und Blattzuordnung hinzufügen
            tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = "mainTable";
            tableLoadOption.TargetSheetIndex = 1;
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            
            // Erneut laden und speichern mit neuen Optionen
            workbook = new Workbook("input.html", loadOptions);
            workbook.Save("output_mapped.xlsx");
        }
    }
}
```

### Siehe auch

* class [HtmlTableLoadOptionCollection](../../htmltableloadoptioncollection/)
* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


