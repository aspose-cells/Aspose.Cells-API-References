---
title: "TableStyleElement.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TableStyleElement‑Eigenschaft. Gibt den Elementtyp zurück"
type: docs
url: /de/net/aspose.cells.tables/tablestyleelement/type/
---
## TableStyleElement.Type property

Liefert den Elementtyp.

```csharp
public TableStyleElementType Type { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableStyleElementPropertyTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten hinzu, um eine Tabelle zu erstellen
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);

            // Eine Tabelle erstellen
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[index];
            table.TableStyleType = TableStyleType.TableStyleMedium9;

            // Den Tabellenstil abrufen (unter Verwendung des Stilnamens anstelle einer Neuerstellung)
            string styleName = table.TableStyleName;
            TableStyle style = workbook.Worksheets.TableStyles[styleName];

            // Auf Tabellestilelemente zugreifen
            TableStyleElement element = style.TableStyleElements[TableStyleElementType.HeaderRow];

            // Anzeige des aktuellen Typs des Elements
            Console.WriteLine("Current Type value: " + element.Type);

            // Hinweis: Die Type-Eigenschaft ist schreibgeschützt, daher können wir sie nicht setzen.
            // element.Type = TableStyleElementType.TotalRow; // Dies würde einen Kompilierungsfehler verursachen

            // Demonstriere, wie verschiedene Elementtypen die Tabelle beeinflussen
            Console.WriteLine("\nAvailable table style elements:");
            foreach (TableStyleElementType type in Enum.GetValues(typeof(TableStyleElementType)))
            {
                try
                {
                    TableStyleElement testElement = style.TableStyleElements[type];
                    Console.WriteLine($"Element type {type} exists in this style");
                }
                catch
                {
                    Console.WriteLine($"Element type {type} not available in this style");
                }
            }

            // Speichere die Arbeitsmappe
            workbook.Save("TableStyleElementTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [TableStyleElementType](../../tablestyleelementtype/)
* class [TableStyleElement](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


