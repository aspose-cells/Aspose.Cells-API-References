---
title: "Cell.SetSharedFormula"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Methode. Setzt eine Formel für einen Zellbereich."
type: docs
url: /de/net/aspose.cells/cell/setsharedformula/
---
## SetSharedFormula(string, int, int, bool, bool) {#setsharedformula_3}

Setzt eine Formel für einen Zellbereich.

```csharp
[Obsolete("Use FormulaParseOptions for more options instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SetSharedFormula(string sharedFormula, int rowNumber, int columnNumber, bool isR1C1, 
    bool isLocal)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sharedFormula | String | Gemeinsame Formel. |
| rowNumber | Int32 | Anzahl der Zeilen, die mit der Formel befüllt werden sollen. |
| columnNumber | Int32 | Anzahl der Spalten, die mit der Formel befüllt werden sollen. |
| isR1C1 | Boolean | ob die Formel eine R1C1-Formel ist |
| isLocal | Boolean | ob die Formel lokalisierungsformatiert ist |

### Hinweise

HINWEIS: Diese Klasse ist jetzt veraltet. Verwenden Sie stattdessen Cell.SetSharedFormula(string,int,int,FormulaParseOptions). Diese Eigenschaft wird 12 Monate nach Dezember 2019 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetSharedFormulaWithStringInt32Int32BooleanBooleanDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe und greife auf das erste Arbeitsblatt zu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            // Beispieldaten in Spalte A befüllen.
            for (int row = 0; row < 5; row++)
            {
                cells[row, 0].Value = row + 1; // A1-A5: 1-5
            }

            // Ermitteln Sie die Zielzelle B1, um die gemeinsame Formel zu setzen.
            Cell targetCell = cells[0, 1]; // B1

            try
            {
                // Setzen Sie die gemeinsame Formel, um das Quadrat der Werte in Spalte A zu berechnen.
                // Parameter: (formula, rowCount=5, columnCount=1, isR1C1=false, isLocal=false)
#pragma warning disable 0618 // Disable obsolete warning for demonstration
                targetCell.SetSharedFormula("=A1^2", 5, 1, false, false);
#pragma warning restore 0618

                // Formelpropagation überprüfen.
                Console.WriteLine($"B1 formula: {targetCell.Formula}");
                Console.WriteLine($"B5 formula: {cells[4, 1].Formula}");

                // Arbeitsmappe berechnen, um Formelergebnisse zu aktualisieren
                workbook.CalculateFormula();

                Console.WriteLine($"A1 value: {cells["A1"].Value}");
                Console.WriteLine($"A5 value: {cells["A5"].Value}");
                Console.WriteLine($"B1 value: {targetCell.Value}");
                Console.WriteLine($"B5 value: {cells[4, 1].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting shared formula: {ex.Message}");
                return;
            }

            // Speichere die geänderte Arbeitsmappe
            workbook.Save("SetSharedFormulaDemo.xlsx");
            Console.WriteLine("Spreadsheet saved successfully.");
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetSharedFormula(string, int, int) {#setsharedformula}

Setzt gemeinsam genutzte Formeln für einen Zellbereich.

```csharp
public void SetSharedFormula(string sharedFormula, int rowNumber, int columnNumber)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sharedFormula | String | Gemeinsame Formel. |
| rowNumber | Int32 | Anzahl der Zeilen, die mit der Formel befüllt werden sollen. |
| columnNumber | Int32 | Anzahl der Spalten, die mit der Formel befüllt werden sollen. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetSharedFormulaWithStringInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Gemeinsame Formel in Spalte B von B1 bis B20 festlegen
            cells["B1"].SetSharedFormula("=C1*2", 20, 1);

            // Einige Werte in Spalte C festlegen, um die Berechnung der Formel zu demonstrieren
            for (int i = 0; i < 20; i++)
            {
                cells[i, 2].PutValue(i + 1); // Column C values (C1=1, C2=2...)
            }

            // Formeln berechnen
            workbook.CalculateFormula();

            // Ergebnisse zur Überprüfung ausgeben
            for (int i = 0; i < 5; i++) // Display first 5 results
            {
                Console.WriteLine($"B{i+1} value: {cells[i, 1].Value}");
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

## SetSharedFormula(string, int, int, FormulaParseOptions) {#setsharedformula_1}

Setzt gemeinsam genutzte Formeln für einen Zellbereich.

```csharp
public void SetSharedFormula(string sharedFormula, int rowNumber, int columnNumber, 
    FormulaParseOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sharedFormula | String | Gemeinsame Formel. |
| rowNumber | Int32 | Anzahl der Zeilen, die mit der Formel befüllt werden sollen. |
| columnNumber | Int32 | Anzahl der Spalten, die mit der Formel befüllt werden sollen. |
| Optionen | FormulaParseOptions | Optionen zum Parsen der Formel. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetSharedFormulaWithStringInt32Int32FormulaParseOpDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe und greife auf das erste Arbeitsblatt zu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten in Spalte A befüllen.
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // Zielzelle abrufen, in der wir die gemeinsame Formel festlegen
            Cell targetCell = worksheet.Cells["B1"];

            try
            {
                // Formel-Parse-Optionen mit Standardeinstellungen erstellen
                FormulaParseOptions options = new FormulaParseOptions();

                // Gemeinsame Formel für 3 Zeilen und 2 Spalten ab B1 festlegen
                targetCell.SetSharedFormula("=A1*2", 3, 2, options);

                Console.WriteLine("Shared formula set successfully for B1:C3 range");
                Console.WriteLine("B1 formula: " + worksheet.Cells["B1"].Formula);
                Console.WriteLine("C3 formula: " + worksheet.Cells["C3"].Formula);

                workbook.CalculateFormula();
                Console.WriteLine("B3 value: " + worksheet.Cells["B3"].Value);
                Console.WriteLine("B1 value: " + worksheet.Cells["B1"].Value);
                Console.WriteLine("C3 value: " + worksheet.Cells["C3"].Value);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting shared formula: {ex.Message}");
            }

            // Speichere die geänderte Arbeitsmappe
            workbook.Save("SetSharedFormulaDemo.xlsx");
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

## SetSharedFormula(string, int, int, FormulaParseOptions, object[][]) {#setsharedformula_2}

Setzt gemeinsam genutzte Formeln für einen Zellbereich.

```csharp
public void SetSharedFormula(string sharedFormula, int rowNumber, int columnNumber, 
    FormulaParseOptions options, object[][] values)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sharedFormula | String | Gemeinsame Formel. |
| rowNumber | Int32 | Anzahl der Zeilen, die mit der Formel befüllt werden sollen. |
| columnNumber | Int32 | Anzahl der Spalten, die mit der Formel befüllt werden sollen. |
| Optionen | FormulaParseOptions | Optionen zum Parsen der Formel. |
| Werte | Object[][] | Werte für diese Zellen mit gegebener gemeinsamer Formel |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellMethodSetSharedFormulaWithStringInt32Int32FormulaParseOpDemo1
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe und greife auf das erste Arbeitsblatt zu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispielwert in Zelle A1 festlegen
            worksheet.Cells["A1"].PutValue(5);

            // Zielzelle B2 abrufen, in der die gemeinsame Formel festgelegt wird
            Cell cell = worksheet.Cells["B2"];

            try
            {
                // Parameter der gemeinsamen Formel definieren
                string formula = "=A1*2";
                int totalRows = 2;
                int totalColumns = 2;
                FormulaParseOptions parseOptions = new FormulaParseOptions();
                object[][] presetValues = new object[2][]
                {
                    new object[] { 10, 10 },
                    new object[] { 10, 10 }
                };

                // Gemeinsame Formel für einen 2x2‑Bereich ab B2 mit voreingestellten Werten festlegen
                cell.SetSharedFormula(formula, totalRows, totalColumns, parseOptions, presetValues);

                Console.WriteLine("Shared formula set successfully. Cells B2:C3 contain values 10");
                workbook.CalculateFormula();
                Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2", "C3");
                IEnumerator iter = range.GetEnumerator();
                while(iter.MoveNext()) 
                {
                    Cell temp = (Cell)iter.Current;
                    Console.WriteLine(temp.Name + "  " + temp.Value);
                }

            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting shared formula: {ex.Message}");
            }

            // Speichere die geänderte Arbeitsmappe
            workbook.Save("SetSharedFormulaDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


