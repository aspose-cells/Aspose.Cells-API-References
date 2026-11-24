---
title: "Name.SetRefersTo"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Name-Methode. Setzt die Referenz dieses Namens"
type: docs
url: /de/net/aspose.cells/name/setrefersto/
---
## Name.SetRefersTo method

Setze die Referenz dieses Namens.

```csharp
public void SetRefersTo(string refersTo, bool isR1C1, bool isLocal)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| refersTo | String | Die Referenz. |
| isR1C1 | Boolean | Ob die Referenz im R1C1-Format vorliegt. |
| isLocal | Boolean | Ob die Referenz nach Gebietsschema formatiert ist. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class NameMethodSetRefersToWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Einige Daten zu den Zellen hinzufügen
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // Benannten Bereich erstellen
            int index = workbook.Worksheets.Names.Add("MyNamedRange");
            Name namedRange = workbook.Worksheets.Names[index];

            try
            {
                // Rufen Sie SetRefersTo mit den Parametern (String, Boolean, Boolean) auf
                namedRange.SetRefersTo("=Sheet1!$A$1:$A$3", false, false);

                // Ergebnis anzeigen
                Console.WriteLine($"Named range 'MyNamedRange' now refers to: {namedRange.RefersTo}");

                // Überprüfen Sie dies, indem Sie den benannten Bereich in einer Formel verwenden
                worksheet.Cells["B1"].Formula = "=SUM(MyNamedRange)";
                workbook.CalculateFormula();

                Console.WriteLine($"Result of SUM(MyNamedRange): {worksheet.Cells["B1"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetRefersTo method: {ex.Message}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("NameMethodSetRefersToWithStringBooleanBooleanDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


