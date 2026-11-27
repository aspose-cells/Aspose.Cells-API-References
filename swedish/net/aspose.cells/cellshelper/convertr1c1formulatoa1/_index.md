---
title: "CellsHelper.ConvertR1C1FormulaToA1"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CellsHelper-metod. Konverterar cellens r1c1-formel till A1-formel"
type: docs
url: /sv/net/aspose.cells/cellshelper/convertr1c1formulatoa1/
---
## CellsHelper.ConvertR1C1FormulaToA1 method

Konverterar cellens r1c1-formel till A1-formel.

```csharp
[Obsolete("Use Worksheet.ConvertFormulaReferenceStyle() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public static string ConvertR1C1FormulaToA1(string r1c1Formula, int row, int column)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| r1c1Formula | String | r1c1-formeln. |
| row | Int32 | Radindex för cellen. |
| column | Int32 | Kolumnindex för cellen. |

### Returvärde

A1-formeln.

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället Worksheet.ConvertFormulaReferenceStyle() metod. Denna egenskap kommer att tas bort 12 månader senare från och med augusti 2023. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodConvertR1C1FormulaToA1WithStringInt32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ange R1C1-formler i celler
            worksheet.Cells["A1"].R1C1Formula = "=R[1]C";
            worksheet.Cells["B1"].R1C1Formula = "=RC[1]";
            worksheet.Cells["A2"].R1C1Formula = "=R2C3";
            worksheet.Cells["B2"].R1C1Formula = "=R[-1]C[-1]";

            // Konvertera R1C1-formler till A1-stil
            string a1Converted = CellsHelper.ConvertR1C1FormulaToA1(worksheet.Cells["A1"].R1C1Formula, 0, 0);
            string b1Converted = CellsHelper.ConvertR1C1FormulaToA1(worksheet.Cells["B1"].R1C1Formula, 0, 0);
            string a2Converted = CellsHelper.ConvertR1C1FormulaToA1(worksheet.Cells["A2"].R1C1Formula, 1, 2);
            string b2Converted = CellsHelper.ConvertR1C1FormulaToA1(worksheet.Cells["B2"].R1C1Formula, 1, 1);

            // Skriv ut resultaten
            Console.WriteLine("A1 R1C1: {0} -> A1: {1}", worksheet.Cells["A1"].R1C1Formula, a1Converted);
            Console.WriteLine("B1 R1C1: {0} -> A1: {1}", worksheet.Cells["B1"].R1C1Formula, b1Converted);
            Console.WriteLine("A2 R1C1: {0} -> A1: {1}", worksheet.Cells["A2"].R1C1Formula, a2Converted);
            Console.WriteLine("B2 R1C1: {0} -> A1: {1}", worksheet.Cells["B2"].R1C1Formula, b2Converted);
        }
    }
}
```

### Se även

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


