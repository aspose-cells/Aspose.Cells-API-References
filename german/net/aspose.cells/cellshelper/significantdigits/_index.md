---
title: "CellsHelper.SignificantDigits"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CellsHelper-Eigenschaft. Gibt die Anzahl signifikanter Stellen zurück und setzt sie. Der Standardwert ist 17"
type: docs
url: /de/net/aspose.cells/cellshelper/significantdigits/
---
## CellsHelper.SignificantDigits property

Gibt die Anzahl signifikanter Stellen zurück und setzt sie. Der Standardwert ist 17.

```csharp
[Obsolete("Use SignificantDigitsType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public static int SignificantDigits { get; set; }
```

### Hinweise

Nur noch 15 oder 17 möglich. HINWEIS: Dieses Mitglied ist jetzt veraltet. Stattdessen verwenden Sie bitte [`SignificantDigitsType`](../significantdigitstype/). Diese Eigenschaft wird 12 Monate später, seit Juni 2025, entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erfahren haben.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperPropertySignificantDigitsDemo
    {
        public static void Run()
        {
            // Signifikante Stellen festlegen
            CellsHelper.SignificantDigits = 15;
            
            // Demonstrieren Sie die Verwendung der Eigenschaft
            Console.WriteLine("Significant Digits: " + CellsHelper.SignificantDigits);
            
            // Erstellen Sie eine Arbeitsmappe, um signifikante Stellen in Berechnungen zu demonstrieren
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Setzen Sie Werte, die von signifikanten Stellen beeinflusst werden
            worksheet.Cells["A1"].PutValue(1.2345678912345678);
            worksheet.Cells["A2"].PutValue(1.2345678912345678);
            worksheet.Cells["A3"].Formula = "=A1+A2";
            
            // Berechnen Sie Formeln mit den festgelegten signifikanten Stellen
            workbook.CalculateFormula();
            
            // Ergebnisse ausgeben
            Console.WriteLine("Value with significant digits: " + worksheet.Cells["A3"].Value);
        }
    }
}
```

### Siehe auch

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


