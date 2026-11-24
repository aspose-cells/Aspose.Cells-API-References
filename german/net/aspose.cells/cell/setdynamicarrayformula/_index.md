---
title: "Cell.SetDynamicArrayFormula"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Methode. Setzt die dynamische Array-Formel und lässt die Formel, falls möglich, in benachbarte Zellen überlaufen."
type: docs
url: /de/net/aspose.cells/cell/setdynamicarrayformula/
---
## SetDynamicArrayFormula(string, FormulaParseOptions, bool) {#setdynamicarrayformula}

Setzt eine dynamische Array-Formel und lässt die Formel, wenn möglich, in benachbarte Zellen überlaufen.

```csharp
public CellArea SetDynamicArrayFormula(string arrayFormula, FormulaParseOptions options, 
    bool calculateValue)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arrayFormula | String | der Formelausdruck |
| Optionen | FormulaParseOptions | Optionen zum Parsen der Formel. Die \"Parse\"-Option wird ignoriert und die Formel wird immer sofort geparst. |
| calculateValue | Boolean | Ob diese dynamische Array-Formel für die Zellen im überlaufenden Bereich berechnet werden soll. |

### Rückgabewert

der Bereich, in den die Formel überlaufen soll.

### Hinweise

Der zurückgegebene Bereich muss nicht mit dem tatsächlichen Bereich übereinstimmen, in den diese dynamische Array-Formel überläuft. Wenn im Bereich nicht leere Zellen vorhanden sind, wird die Formel nur für die aktuelle Zelle gesetzt und mit \"#SPILL!\" markiert. In einem solchen Fall geben wir jedoch weiterhin den gesamten Bereich zurück, in den die Formel überlaufen sollte.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetDynamicArrayFormulaWithStringFormulaParseOptionsBooleDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Setze die dynamische Array-Formel in Zelle A1
            Cell cell1 = cells["A1"];
            cell1.SetDynamicArrayFormula("=SEQUENCE(B2)", new FormulaParseOptions(), true);

            // Setze den Wert in B2, der die SEQUENCE-Formel beeinflusst
            cells["B2"].PutValue(3);

            // Formeln berechnen und dynamische Arrays aktualisieren
            wb.CalculateFormula();
            wb.RefreshDynamicArrayFormulas(false);

            // Gib die Ergebnisse aus dem überlaufenden Bereich aus
            Console.WriteLine("Dynamic array results:");
            for (int i = 0; i < 3; i++)
            {
                Console.WriteLine(cells[0, i].Value);
            }
        }
    }
}
```

### Siehe auch

* struct [CellArea](../../cellarea/)
* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDynamicArrayFormula(string, FormulaParseOptions, object[][], bool, bool) {#setdynamicarrayformula_1}

Setzt eine dynamische Array-Formel und lässt die Formel, wenn möglich, in benachbarte Zellen überlaufen.

```csharp
public CellArea SetDynamicArrayFormula(string arrayFormula, FormulaParseOptions options, 
    object[][] values, bool calculateRange, bool calculateValue)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arrayFormula | String | der Formelausdruck |
| Optionen | FormulaParseOptions | Optionen zum Parsen der Formel. Die \"Parse\"-Option wird ignoriert und die Formel wird immer sofort geparst. |
| Werte | Object[][] | Werte (berechnete Ergebnisse) für die Zellen mit der angegebenen dynamischen Array-Formel |
| calculateRange | Boolean | Ob der überlaufende Bereich für diese dynamische Array-Formel berechnet werden soll. Wenn der Parameter \"values\" nicht null ist und dieses Flag false ist, wird die Höhe des überlaufenden Bereichs values.Length und die Breite values[0].Length sein. |
| calculateValue | Boolean | ob diese dynamische Array-Formel für die Zellen im ausgegebenen Bereich berechnet wird, wenn "values" null ist oder das entsprechende Element in "values" für eine Zelle null ist. |

### Rückgabewert

der Bereich, in den die Formel überlaufen soll.

### Hinweise

Der zurückgegebene Bereich muss nicht mit dem tatsächlichen Bereich übereinstimmen, in den diese dynamische Array-Formel überläuft. Wenn im Bereich nicht leere Zellen vorhanden sind, wird die Formel nur für die aktuelle Zelle gesetzt und mit \"#SPILL!\" markiert. In einem solchen Fall geben wir jedoch weiterhin den gesamten Bereich zurück, in den die Formel überlaufen sollte.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetDynamicArrayFormulaWithStringFormulaParseOptionsObjecDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            Cell cell = cells["A1"];
            cell.PutValue(10);
            cell = cells["A2"];
            cell.PutValue(20);
            cell = cells["B1"];
            cell.PutValue(60);
            cell = cells["B2"];
            cell.PutValue(80);

            // Hole die Zelle C1, in der die dynamische Array-Formel gesetzt wird.
            cell = worksheet.Cells["C1"];

            // Definiere die dynamische Array-Formel
            string formula = "=A1:B2 * 2";
            
            // Erstelle Optionen zum Parsen der Formel
            FormulaParseOptions options = new FormulaParseOptions
            {
                Parse = true // Enable formula parsing
            };

            // Bereite Werte vor, um die Ergebniszellen der Formel zu füllen
            object[][] values = new object[2][];
            values[0] = new object[] { 2, 4 };
            values[1] = new object[] { 6, 8 };

            try
            {
                // Setze die dynamische Array-Formel mit vorab berechneten Werten
                CellArea result = cell.SetDynamicArrayFormula(
                    formula,
                    options,
                    values,
                    calculateRange: false,  // Use values array dimensions for spill range
                    calculateValue: false  // Use provided values instead of calculating
                );

                Console.WriteLine($"Dynamic array formula set. Affected range: Rows {result.StartRow}-{result.EndRow}, Columns {result.StartColumn}-{result.EndColumn}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetDynamicArrayFormula: {ex.Message}");
            }

            // Speichere die Arbeitsmappe mit den Änderungen
            workbook.Save("SetDynamicArrayFormulaDemo.xlsx");
        }
    }
}
```

### Siehe auch

* struct [CellArea](../../cellarea/)
* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDynamicArrayFormula(string, FormulaParseOptions, object[][], bool, bool, CalculationOptions) {#setdynamicarrayformula_2}

Setzt eine dynamische Array-Formel und lässt die Formel, wenn möglich, in benachbarte Zellen überlaufen.

```csharp
public CellArea SetDynamicArrayFormula(string arrayFormula, FormulaParseOptions options, 
    object[][] values, bool calculateRange, bool calculateValue, CalculationOptions copts)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arrayFormula | String | der Formelausdruck |
| Optionen | FormulaParseOptions | Optionen zum Parsen der Formel. Die \"Parse\"-Option wird ignoriert und die Formel wird immer sofort geparst. |
| Werte | Object[][] | Werte (berechnete Ergebnisse) für die Zellen mit der angegebenen dynamischen Array-Formel |
| calculateRange | Boolean | Ob der überlaufende Bereich für diese dynamische Array-Formel berechnet werden soll. Wenn der Parameter \"values\" nicht null ist und dieses Flag false ist, wird die Höhe des überlaufenden Bereichs values.Length und die Breite values[0].Length sein. |
| calculateValue | Boolean | ob diese dynamische Array-Formel für die Zellen im ausgegebenen Bereich berechnet wird, wenn "values" null ist oder das entsprechende Element in "values" für eine Zelle null ist. |
| copts | CalculationOptions | Die Optionen zur Berechnung der Formel. In der Regel sollte aus Leistungsgründen die [`Recursive`](../../calculationoptions/recursive/)‑Eigenschaft auf false gesetzt werden. |

### Rückgabewert

der Bereich, in den die Formel überlaufen soll.

### Hinweise

Der zurückgegebene Bereich muss nicht mit dem tatsächlichen Bereich übereinstimmen, in den diese dynamische Array-Formel überläuft. Wenn im Bereich nicht leere Zellen vorhanden sind, wird die Formel nur für die aktuelle Zelle gesetzt und mit \"#SPILL!\" markiert. In einem solchen Fall geben wir jedoch weiterhin den gesamten Bereich zurück, in den die Formel überlaufen sollte.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetDynamicArrayFormulaWithStringFormulaParseOptionsObjecDemo1
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fülle Beispiel-Daten in die Zellen A2:B5 ein
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(60);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["B3"].PutValue(55);
            worksheet.Cells["A4"].PutValue(30);
            worksheet.Cells["B4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(40);
            worksheet.Cells["B5"].PutValue(70);

            // Hole die Zielzelle D1
            Cell cellD1 = worksheet.Cells["D1"];

            try
            {
                // Bereite Parameter für SetDynamicArrayFormula vor
                string formula = "=FILTER(A2:A5, B2:B5>50)";
                FormulaParseOptions options = new FormulaParseOptions { Parse = true };
                object[][] values = new object[2][] { new object[] { 10 }, new object[] { 40 } };
                bool calculateRange = true;
                bool calculateValue = true;
                CalculationOptions calcOptions = new CalculationOptions { Recursive = true };

                // Rufe SetDynamicArrayFormula mit spezifischen Parametern auf
                CellArea spillRange = cellD1.SetDynamicArrayFormula(
                    formula,
                    options,
                    values,
                    calculateRange,
                    calculateValue,
                    calcOptions
                );

                Console.WriteLine($"Dynamic array formula set successfully. Spill range: {spillRange}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetDynamicArrayFormula method: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("SetDynamicArrayFormulaDemo.xlsx");
        }
    }
}
```

### Siehe auch

* struct [CellArea](../../cellarea/)
* class [FormulaParseOptions](../../formulaparseoptions/)
* class [CalculationOptions](../../calculationoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


