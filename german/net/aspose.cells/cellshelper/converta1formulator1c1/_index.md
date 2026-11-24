---
title: "CellsHelper.ConvertA1FormulaToR1C1"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CellsHelper-Methode. Konvertiert die A1-Formel der Zelle in die R1C1-Formel"
type: docs
url: /de/net/aspose.cells/cellshelper/converta1formulator1c1/
---
## CellsHelper.ConvertA1FormulaToR1C1 method

Konvertiert die A1-Formel der Zelle in die R1C1-Formel.

```csharp
[Obsolete("Use Worksheet.ConvertFormulaReferenceStyle() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public static string ConvertA1FormulaToR1C1(string formula, int row, int column)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Formel | String | Die A1-Formel. |
| row | Int32 | Der Zeilenindex der Zelle. |
| column | Int32 | Der Spaltenindex der Zelle. |

### Rückgabewert

Die R1C1-Formel.

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Methode Worksheet.ConvertFormulaReferenceStyle(). Diese Eigenschaft wird 12 Monate nach August 2023 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodConvertA1FormulaToR1C1WithStringInt32Int32Demo
    {
        public static void Run()
        {
            // Konvertieren Sie die A1-Formel in den R1C1-Stil
            string r1c1Formula = CellsHelper.ConvertA1FormulaToR1C1("=A1+B2", 0, 0);
            Console.WriteLine("R1C1 Formula: " + r1c1Formula);
        }
    }
}
```

### Siehe auch

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


