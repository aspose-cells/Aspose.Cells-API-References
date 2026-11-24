---
title: "FormatCondition.SetFormulas"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FormatCondition-Methode. Legt den Wert oder Ausdruck fest, der mit dieser Formatbedingung verknüpft ist"
type: docs
url: /de/net/aspose.cells/formatcondition/setformulas/
---
## FormatCondition.SetFormulas method

Setzt den Wert oder Ausdruck, der mit dieser Formatierungsbedingung verknüpft ist.

```csharp
public void SetFormulas(string formula1, string formula2, bool isR1C1, bool isLocal)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| formula1 | String | Der Wert oder Ausdruck, der mit dieser Formatbedingung verknüpft ist. Wenn der Eingabewert mit '=' beginnt, wird er als Formel behandelt. Andernfalls wird er als einfacher Wert (Text, Zahl, Bool) interpretiert. Für Textwerte, die mit '=', beginnen, kann der Benutzer ihn im Format "=\"=...\"" als Formel eingeben. |
| formula2 | String | Der Wert oder Ausdruck, der mit dieser Formatbedingung verknüpft ist. Das Eingabeformat ist dasselbe wie bei Formula1. |
| isR1C1 | Boolean | Ob die Formel eine R1C1-Formel ist. |
| isLocal | Boolean | Ob die Formel lokalisierungsabhängig formatiert ist. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionMethodSetFormulasWithStringStringBooleanBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            ConditionalFormattingCollection cfs = worksheet.ConditionalFormattings;
            int formatIndex = cfs.Add();
            FormatConditionCollection fcs = cfs[formatIndex];
            
            fcs.AddArea(CellArea.CreateCellArea("A1", "C10"));
            
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue);
            FormatCondition fc = fcs[conditionIndex];
            
            fc.Operator = OperatorType.Between;
            fc.SetFormulas("=1", "=2", false, false);
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


