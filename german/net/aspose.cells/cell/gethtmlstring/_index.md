---
title: "Cell.GetHtmlString"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Methode. Gibt den HTML-String zurück, der Daten und einige Formate in dieser Zelle enthält"
type: docs
url: /de/net/aspose.cells/cell/gethtmlstring/
---
## Cell.GetHtmlString method

Liefert den HTML-String, der Daten und einige Formate in dieser Zelle enthält.

```csharp
public string GetHtmlString(bool html5)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| html5 | Boolean | Gibt an, ob der Wert mit html5 kompatibel ist |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetHtmlStringWithBooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Setzen Sie einen Beispielzellenwert mit Formatierung
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");
            Style style = cell.GetStyle();
            style.Font.Name = "Calibri";
            style.Font.Size = 11;
            style.Font.Color = System.Drawing.Color.Red;
            cell.SetStyle(style);

            // Demonstrieren Sie GetHtmlString mit booleschem Parameter
            string htmlWithoutDiv = cell.GetHtmlString(false);
            string htmlWithDiv = cell.GetHtmlString(true);
            
            Console.WriteLine("HTML without div wrapper:");
            Console.WriteLine(htmlWithoutDiv);
            Console.WriteLine("\nHTML with div wrapper:");
            Console.WriteLine(htmlWithDiv);
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


