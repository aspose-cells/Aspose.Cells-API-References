---
title: "Style.IsPercent"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Style-Eigenschaft. Gibt an, ob das Zahlenformat ein Prozentformat ist"
type: docs
url: /de/net/aspose.cells/style/ispercent/
---
## Style.IsPercent property

Gibt an, ob das Zahlenformat ein Prozentformat ist.

```csharp
public bool IsPercent { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StylePropertyIsPercentDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Greife auf Zelle A1 zu und setze ihren Wert
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue(0.5);
            
            // Ermitteln Sie den Stil der Zelle
            Style style = cell.GetStyle();
            
            // Zeige den aktuellen IsPercent-Wert an
            Console.WriteLine("Current IsPercent value: " + style.IsPercent);
            
            // Setze das Zahlenformat auf Prozent (dies setzt IsPercent automatisch auf true)
            style.Number = 10; // 10 is the built-in percentage format in Excel
            
            // Wenden Sie den Stil auf die Zelle an
            cell.SetStyle(style);
            
            // Überprüfe, dass IsPercent jetzt true ist
            Console.WriteLine("After setting percentage format, IsPercent value: " + style.IsPercent);
            
            // Erstelle eine weitere Zelle mit anderem Format
            Cell cell2 = worksheet.Cells["A2"];
            cell2.PutValue(0.75);
            Style style2 = cell2.GetStyle();
            style2.Number = 3; // 3 is the built-in number format (not percentage)
            cell2.SetStyle(style2);
            
            // Überprüfe, dass IsPercent für ein Nicht-Prozentformat false ist
            Console.WriteLine("For non-percentage format, IsPercent value: " + style2.IsPercent);
            
            // Speichere die Arbeitsmappe
            workbook.Save("StylePropertyIsPercentDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


