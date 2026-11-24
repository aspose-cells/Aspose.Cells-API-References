---
title: "Cell.StringValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Eigenschaft. Gibt den Zeichenkettenwert zurück, der in der Zelle enthalten ist. Wenn der Typ dieser Zelle Zeichenkette ist, wird der Zeichenkettenwert selbst zurückgegeben. Für andere Zellentypen wird der formatierte Zeichenkettenwert zurückgegeben, der mit dem angegebenen Stil dieser Zelle formatiert ist. Der formatierte Zellenwert entspricht dem, was Sie aus Excel erhalten, wenn Sie eine Zelle als Text kopieren, z. B. beim Kopieren der Zelle in einen Texteditor oder beim Exportieren in CSV."
type: docs
url: /de/net/aspose.cells/cell/stringvalue/
---
## Cell.StringValue property

Ermittelt den Zeichenkettenwert, der in der Zelle enthalten ist. Wenn der Typ dieser Zelle Zeichenkette ist, wird der Zeichenkettenwert selbst zurückgegeben. Für andere Zellentypen wird der formatierte Zeichenkettenwert (formatiert mit dem angegebenen Stil dieser Zelle) zurückgegeben. Der formatierte Zellenwert entspricht dem, was Sie aus Excel erhalten, wenn Sie eine Zelle als Text kopieren (z. B. das Kopieren einer Zelle in einen Texteditor oder das Exportieren nach CSV).

```csharp
public string StringValue { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyStringValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Setzen Sie einige Werte
            cells["A1"].PutValue("Hello");
            cells["A2"].PutValue(123);
            cells["A3"].PutValue(DateTime.Now);
            cells["A4"].Formula = "=A1&A2";

            // Formeln berechnen
            workbook.CalculateFormula();

            // Demonstrieren Sie die StringValue-Eigenschaft
            Console.WriteLine("A1 StringValue: " + cells["A1"].StringValue);
            Console.WriteLine("A2 StringValue: " + cells["A2"].StringValue);
            Console.WriteLine("A3 StringValue: " + cells["A3"].StringValue);
            Console.WriteLine("A4 StringValue: " + cells["A4"].StringValue);

            // Fehlerwertfall anzeigen
            Cell errorCell = cells["B1"];
            errorCell.Formula = "=1/0";
            workbook.CalculateFormula();
            Console.WriteLine("B1 (Error) StringValue: " + errorCell.StringValue);
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


