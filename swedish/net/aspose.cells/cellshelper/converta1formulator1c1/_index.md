---
title: "CellsHelper.ConvertA1FormulaToR1C1"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CellsHelper-metod. Konverterar A1-formeln för cellen till r1c1-formeln"
type: docs
url: /sv/net/aspose.cells/cellshelper/converta1formulator1c1/
---
## CellsHelper.ConvertA1FormulaToR1C1 method

Konverterar A1-formeln för cellen till r1c1-formeln.

```csharp
[Obsolete("Use Worksheet.ConvertFormulaReferenceStyle() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public static string ConvertA1FormulaToR1C1(string formula, int row, int column)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| formel | String | A1-formeln. |
| row | Int32 | Radindex för cellen. |
| column | Int32 | Kolumnindex för cellen. |

### Returvärde

R1C1-formeln.

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället Worksheet.ConvertFormulaReferenceStyle() metod. Denna egenskap kommer att tas bort 12 månader senare från och med augusti 2023. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodConvertA1FormulaToR1C1WithStringInt32Int32Demo
    {
        public static void Run()
        {
            // Konvertera A1-stilsformel till R1C1-stil
            string r1c1Formula = CellsHelper.ConvertA1FormulaToR1C1("=A1+B2", 0, 0);
            Console.WriteLine("R1C1 Formula: " + r1c1Formula);
        }
    }
}
```

### Se även

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


