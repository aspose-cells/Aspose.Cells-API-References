---
title: "FormatCondition.SetFormula2"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FormatCondition-Methode. Legt den Wert oder Ausdruck fest, der mit dieser Formatbedingung verknüpft ist"
type: docs
url: /de/net/aspose.cells/formatcondition/setformula2/
---
## FormatCondition.SetFormula2 method

Setzt den Wert oder Ausdruck, der mit dieser Formatierungsbedingung verknüpft ist.

```csharp
public void SetFormula2(string formula, bool isR1C1, bool isLocal)
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

    public class FormatConditionMethodSetFormula2WithStringBooleanBooleanDemo
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

            // Füge eine Formatierungsbedingung hinzu
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 3;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "30");

            // Holen Sie die erste Formatbedingung
            FormatCondition fc = fcs[0];

            try
            {
                // Rufen Sie SetFormula2 mit den Parametern (String, Boolean, Boolean) auf
                fc.SetFormula2("25", false, false);

                // Ergebnis anzeigen
                Console.WriteLine("SetFormula2 executed successfully. New Formula2: " + fc.Formula2);
                Console.WriteLine("Cells A1:A4 will be formatted if their values are between 10 and 25");

                // Wenden Sie einen Stil an, um die Wirkung sichtbar zu machen
                Style style = workbook.CreateStyle();
                style.BackgroundColor = System.Drawing.Color.LightGreen;
                fc.Style = style;
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFormula2 method: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("FormatConditionSetFormula2Demo.xlsx");
        }
    }
}
```

### Siehe auch

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


