---
title: "FormatCondition.SetFormula1"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FormatCondition-Methode. Legt den Wert oder Ausdruck fest, der mit dieser Formatbedingung verknüpft ist"
type: docs
url: /de/net/aspose.cells/formatcondition/setformula1/
---
## FormatCondition.SetFormula1 method

Setzt den Wert oder Ausdruck, der mit dieser Formatierungsbedingung verknüpft ist.

```csharp
public void SetFormula1(string formula, bool isR1C1, bool isLocal)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Formel | String | Der Wert oder Ausdruck, der mit dieser Formatbedingung verknüpft ist. Wenn der Eingabewert mit '=' beginnt, wird er als Formel behandelt. Andernfalls wird er als einfacher Wert (Text, Zahl, Bool) interpretiert. Für Textwerte, die mit '=', beginnen, kann der Benutzer ihn im Format "=\"=...\"" als Formel eingeben. |
| isR1C1 | Boolean | Ob die Formel eine R1C1-Formel ist. |
| isLocal | Boolean | Ob die Formel lokalisierungsabhängig formatiert ist. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormatConditionMethodSetFormula1WithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Fügen Sie einen Bereich für bedingte Formatierung hinzu
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 3;
            area.EndColumn = 0;
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "30");

            // Holen Sie die erste Formatbedingung
            FormatCondition fc = fcc[0];

            try
            {
                // Rufen Sie SetFormula1 mit den Parametern (String, Boolean, Boolean) auf
                fc.SetFormula1("SUM(A1:A4)", false, false);

                // Ergebnis anzeigen
                Console.WriteLine("SetFormula1 executed successfully with formula: " + fc.Formula1);
                Console.WriteLine("Conditional formatting applied to range A1:A4 with formula: " + fc.Formula1);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFormula1 method: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("FormatConditionSetFormula1Demo.xlsx");
        }
    }
}
```

### Siehe auch

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


