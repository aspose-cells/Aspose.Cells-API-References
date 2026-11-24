---
title: "Cell.NumberCategoryType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell‑Eigenschaft. Gibt den Kategorietyp der Zahlenformatierung dieser Zelle an"
type: docs
url: /de/net/aspose.cells/cell/numbercategorytype/
---
## Cell.NumberCategoryType property

Stellt den Kategorie‑Typ der Zahlenformatierung dieser Zelle dar.

```csharp
public NumberCategoryType NumberCategoryType { get; }
```

### Hinweise

Wenn das Formatierungsmuster einer Zelle mit bedingten Formatierungsmustern kombiniert wird, entspricht der zurückgegebene Typ dem Teil, der für den aktuellen Wert dieser Zelle verwendet wird. Zum Beispiel, wenn das Formatierungsmuster für diese Zelle "#,##0;(#,##0);"-";@" ist, dann ist der zurückgegebene Typ Number, wenn der Zellenwert numerisch und nicht 0 ist; ist der Zellenwert 0 oder kein numerischer Wert, ist der zurückgegebene Typ Text.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyNumberCategoryTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge einen Datumswert zu Zelle A1 hinzu
            Cell dateCell = worksheet.Cells["A1"];
            dateCell.PutValue(DateTime.Now);
            
            // Setze das Datumsformat
            Style dateStyle = dateCell.GetStyle();
            dateStyle.Custom = "yyyy-mm-dd";
            dateCell.SetStyle(dateStyle);
            
            // Füge einen numerischen Wert zu Zelle A2 hinzu
            Cell numberCell = worksheet.Cells["A2"];
            numberCell.PutValue(1234.56);
            
            // Füge einen Textwert zu Zelle A3 hinzu
            Cell textCell = worksheet.Cells["A3"];
            textCell.PutValue("Sample Text");
            
            // Zeige NumberCategoryType für jede Zelle an
            Console.WriteLine("A1 (Date) NumberCategoryType: " + dateCell.NumberCategoryType);
            Console.WriteLine("A2 (Number) NumberCategoryType: " + numberCell.NumberCategoryType);
            Console.WriteLine("A3 (Text) NumberCategoryType: " + textCell.NumberCategoryType);
            
            // Ändern Sie A2 in das Währungsformat und prüfen Sie NumberCategoryType
            Style currencyStyle = numberCell.GetStyle();
            currencyStyle.Custom = "$#,##0.00";
            numberCell.SetStyle(currencyStyle);
            Console.WriteLine("A2 (Currency) NumberCategoryType: " + numberCell.NumberCategoryType);
        }
    }
}
```

### Siehe auch

* enum [NumberCategoryType](../../numbercategorytype/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


