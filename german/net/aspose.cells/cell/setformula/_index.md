---
title: "Cell.SetFormula"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Methode. Setzen Sie die Formel und das berechnete Ergebnis der Formel"
type: docs
url: /de/net/aspose.cells/cell/setformula/
---
## SetFormula(string, object) {#setformula_3}

Setzt die Formel und den Wert (berechnetes Ergebnis) der Formel.

```csharp
public void SetFormula(string formula, object value)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Formel | String | Die Formel. |
| Wert | Object | Der Wert (berechnetes Ergebnis) der Formel. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetFormulaWithStringObjectDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Formel mit Zeichenketten- und Objektparametern festlegen
            cells["A1"].SetFormula("=SUM(1,2)", 4); // Will display 4 until calculation
            cells["A2"].SetFormula("=AVERAGE(5,10)", 7.5); // Will display 7.5 until calculation

            // Werte vor der Berechnung anzeigen
            Console.WriteLine("Before Calculation:");
            Console.WriteLine("A1: " + cells["A1"].StringValue);
            Console.WriteLine("A2: " + cells["A2"].StringValue);

            // Formeln berechnen
            workbook.CalculateFormula();

            // Werte nach der Berechnung anzeigen
            Console.WriteLine("\nAfter Calculation:");
            Console.WriteLine("A1: " + cells["A1"].IntValue); // Should show 3
            Console.WriteLine("A2: " + cells["A2"].DoubleValue); // Should show 7.5
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetFormula(string, FormulaParseOptions) {#setformula}

Setzt die Formel und den Wert (berechnetes Ergebnis) der Formel.

```csharp
public void SetFormula(string formula, FormulaParseOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Formel | String | Die Formel. |
| Optionen | FormulaParseOptions | Optionen zum Parsen der Formel. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetFormulaWithStringFormulaParseOptionsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Eine bestimmte Zelle abrufen (in diesem Fall B2)
            Cell cell = worksheet.Cells["B2"];
            
            // Einige Anfangswerte zur Demonstration festlegen
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["B1"].PutValue(30);
            
            // Beispiel 1: Eine einfache Formel mit Standard‑Parse‑Optionen festlegen
            cell.SetFormula("=SUM(A1:A2)", new FormulaParseOptions());
            Console.WriteLine("Formula with default options: " + cell.Formula);
            
            // Beispiel 2: Formel im R1C1-Stil mit FormulaParseOptions festlegen
            FormulaParseOptions options = new FormulaParseOptions();
            options.Parse = true;
            options.R1C1Style = true;
            
            cell.SetFormula("=SUM(R[-1]C[-1]:R[0]C[-1])", options);
            Console.WriteLine("Formula with R1C1 style: " + cell.Formula);
            
            // Beispiel 3: Formel mit Parse‑Optionen festlegen, die das R1C1-Format beibehalten
            options = new FormulaParseOptions();
            options.Parse = true;
            options.R1C1Style = true;
            cell.SetFormula("=R1C1+R2C2", options);
            Console.WriteLine("Formula preserved as R1C1: " + cell.Formula);
            
            // Berechnen Sie die Arbeitsmappe, um die Ergebnisse zu sehen
            workbook.CalculateFormula();
            Console.WriteLine("Calculated value: " + cell.Value);
        }
    }
}
```

### Siehe auch

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetFormula(string, bool, bool, object) {#setformula_2}

Setzt die Formel und den Wert der Formel.

```csharp
[Obsolete("Use FormulaParseOptions for more options instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SetFormula(string formula, bool isR1C1, bool isLocal, object value)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Formel | String | Die Formel. |
| isR1C1 | Boolean | Ob die Formel eine R1C1-Formel ist. |
| isLocal | Boolean | Ob die Formel lokalisierungsabhängig formatiert ist. |
| Wert | Object | Der Wert der Formel. |

### Hinweise

HINWEIS: Diese Klasse ist jetzt veraltet. Verwenden Sie stattdessen Cell.SetFormula(string,FormulaParseOptions,object). Diese Eigenschaft wird 12 Monate später, seit Dezember 2019, entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetFormulaWithStringBooleanBooleanObjectDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["B1"].PutValue(30);
            worksheet.Cells["B2"].PutValue(40);

            // Die Zielzelle abrufen, in der wir die Formel setzen werden
            Cell cell = worksheet.Cells["C1"];

            try
            {
                // Formel mit allen Parametern festlegen
                // Parameter: Formelzeichenkette, isR1C1, isLocal, Wert
                cell.SetFormula("=SUM(A1:B2)", false, false, null);

                // Formel berechnen
                workbook.CalculateFormula();

                // Ergebnis anzeigen
                Console.WriteLine($"Formula set successfully. Result: {cell.Value}");

                // Speichere die Arbeitsmappe
                workbook.Save("SetFormulaDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting formula: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetFormula(string, FormulaParseOptions, object) {#setformula_1}

Setzt die Formel und den Wert (berechnetes Ergebnis) der Formel.

```csharp
public void SetFormula(string formula, FormulaParseOptions options, object value)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Formel | String | Die Formel. |
| Optionen | FormulaParseOptions | Optionen zum Parsen der Formel. |
| Wert | Object | Der Wert (berechnetes Ergebnis) der Formel. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetFormulaWithStringFormulaParseOptionsObjecDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // Anfängliche Formel mit Add‑In‑Verweis festlegen
            sheet.Cells[0, 0].Formula = "'externalDS.xlam'!dsfun(B1)";
            Console.WriteLine("Initial formula: " + sheet.Cells[0, 0].Formula);

            // Verwenden Sie SetFormula, um ohne Überprüfung des Add‑Ins zu überschreiben
            sheet.Cells[0, 0].SetFormula("=dsfun(B1)", new FormulaParseOptions() { CheckAddIn = false }, null);
            Console.WriteLine("After SetFormula: " + sheet.Cells[0, 0].Formula);

            // Zurücksetzen auf Add‑In‑Formel
            sheet.Cells[0, 0].Formula = "'externalDS.xlam'!dsfun(B1)";
            Console.WriteLine("Reset to add-in formula: " + sheet.Cells[0, 0].Formula);

            // Neue Arbeitsmappe erstellen und Blatt kopieren
            Workbook wb2 = new Workbook();
            wb2.Worksheets[0].Cells[0, 0].Formula = "'externalDS.xlam'!dsfunnew(C1)";
            wb2.Worksheets[0].Copy(sheet);
            Console.WriteLine("After copy: " + wb2.Worksheets[0].Cells[0, 0].Formula);
        }
    }
}
```

### Siehe auch

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


