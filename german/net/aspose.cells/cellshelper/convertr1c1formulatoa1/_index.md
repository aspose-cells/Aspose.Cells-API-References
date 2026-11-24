---
title: "CellsHelper.ConvertR1C1FormulaToA1"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CellsHelper-Methode. Konvertiert die r1c1-Formel der Zelle in die A1-Formel"
type: docs
url: /de/net/aspose.cells/cellshelper/convertr1c1formulatoa1/
---
## CellsHelper.ConvertR1C1FormulaToA1 method

Konvertiert die r1c1-Formel der Zelle in die A1-Formel.

```csharp
[Obsolete("Use Worksheet.ConvertFormulaReferenceStyle() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public static string ConvertR1C1FormulaToA1(string r1c1Formula, int row, int column)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| r1c1Formula | String | Die r1c1-Formel. |
| row | Int32 | Der Zeilenindex der Zelle. |
| column | Int32 | Der Spaltenindex der Zelle. |

### Rückgabewert

Die A1-Formel.

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Methode Worksheet.ConvertFormulaReferenceStyle(). Diese Eigenschaft wird 12 Monate nach August 2023 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodConvertR1C1FormulaToA1WithStringInt32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // R1C1-Formeln in Zellen festlegen
            worksheet.Cells["A1"].R1C1Formula = "=R[1]C";
            worksheet.Cells["B1"].R1C1Formula = "=RC[1]";
            worksheet.Cells["A2"].R1C1Formula = "=R2C3";
            worksheet.Cells["B2"].R1C1Formula = "=R[-1]C[-1]";

            // R1C1-Formeln in den A1-Stil konvertieren
            string a1Converted = CellsHelper.ConvertR1C1FormulaToA1(worksheet.Cells["A1"].R1C1Formula, 0, 0);
            string b1Converted = CellsHelper.ConvertR1C1FormulaToA1(worksheet.Cells["B1"].R1C1Formula, 0, 0);
            string a2Converted = CellsHelper.ConvertR1C1FormulaToA1(worksheet.Cells["A2"].R1C1Formula, 1, 2);
            string b2Converted = CellsHelper.ConvertR1C1FormulaToA1(worksheet.Cells["B2"].R1C1Formula, 1, 1);

            // Ergebnisse ausgeben
            Console.WriteLine("A1 R1C1: {0} -> A1: {1}", worksheet.Cells["A1"].R1C1Formula, a1Converted);
            Console.WriteLine("B1 R1C1: {0} -> A1: {1}", worksheet.Cells["B1"].R1C1Formula, b1Converted);
            Console.WriteLine("A2 R1C1: {0} -> A1: {1}", worksheet.Cells["A2"].R1C1Formula, a2Converted);
            Console.WriteLine("B2 R1C1: {0} -> A1: {1}", worksheet.Cells["B2"].R1C1Formula, b2Converted);
        }
    }
}
```

### Siehe auch

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


