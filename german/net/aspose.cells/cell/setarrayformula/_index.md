---
title: "Cell.SetArrayFormula"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Methode. Setzt eine Array-Formel für einen Zellbereich"
type: docs
url: /de/net/aspose.cells/cell/setarrayformula/
---
## SetArrayFormula(string, int, int, bool, bool) {#setarrayformula_3}

Setzt eine Array-Formel für einen Zellbereich.

```csharp
[Obsolete("Use FormulaParseOptions for more options instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SetArrayFormula(string arrayFormula, int rowNumber, int columnNumber, bool isR1C1, 
    bool isLocal)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arrayFormula | String | Array-Formel. |
| rowNumber | Int32 | Anzahl der Zeilen, um das Ergebnis der Array-Formel zu füllen. |
| columnNumber | Int32 | Anzahl der Spalten, um das Ergebnis der Array-Formel zu füllen. |
| isR1C1 | Boolean | ob die Formel eine R1C1-Formel ist |
| isLocal | Boolean | ob die Formel lokalisierungsformatiert ist |

### Hinweise

HINWEIS: Diese Klasse ist jetzt veraltet. Verwenden Sie stattdessen Cell.SetArrayFormula(string,int,int,FormulaParseOptions). Diese Eigenschaft wird 12 Monate später, seit Dezember 2019, entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetArrayFormulaWithStringInt32Int32BooleanBooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten hinzu
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Value = 20;
            worksheet.Cells["A3"].Value = 30;

            try
            {
                // Erhalte die Zielzelle, in der wir die Array-Formel setzen wollen
                Cell targetCell = worksheet.Cells["B1"];

                // Setze eine Array-Formel, die die Werte in A1:A3 mit 2 multipliziert
                // Parameter: (formula, rowNumber=3, columnNumber=1, isR1C1=false, isLocal=false)
                targetCell.SetArrayFormula("=A1:A3*2", 3, 1, false, false);

                // Berechne die Arbeitsmappe, um die Ergebnisse zu sehen
                workbook.CalculateFormula();

                // Ergebnisse anzeigen
                Console.WriteLine($"B1 value: {targetCell.Value}");
                Console.WriteLine($"B2 value: {worksheet.Cells["B2"].Value}");
                Console.WriteLine($"B3 value: {worksheet.Cells["B3"].Value}");

                // Speichere die Arbeitsmappe
                workbook.Save("SetArrayFormulaDemo.xlsx");
                Console.WriteLine("Array formula set successfully and workbook saved.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting array formula: {ex.Message}");
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

## SetArrayFormula(string, int, int) {#setarrayformula}

Setzt eine Array-Formel (Legacy-Array-Formel, die in MS Excel über STRG+SHIFT+ENTER eingegeben wird) für einen Zellbereich.

```csharp
public void SetArrayFormula(string arrayFormula, int rowNumber, int columnNumber)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arrayFormula | String | Array-Formel. |
| rowNumber | Int32 | Anzahl der Zeilen, um das Ergebnis der Array-Formel zu füllen. |
| columnNumber | Int32 | Anzahl der Spalten, um das Ergebnis der Array-Formel zu füllen. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetArrayFormulaWithStringInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            Cell cell = cells["A1"];
            cell.SetArrayFormula("=FREQUENCY({\"79\",\"85\",\"78\",\"85\",\"50\",\"81\",\"95\",\"88\",\"97\"},{70,79,89})", 4, 1);

            workbook.CalculateFormula();

            for (int i = 0; i < 4; i++)
            {
                Console.WriteLine($"Cell A{i+1} value: {cells[i, 0].IntValue}");
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

## SetArrayFormula(string, int, int, FormulaParseOptions) {#setarrayformula_1}

Setzt eine Array-Formel für einen Zellbereich.

```csharp
public void SetArrayFormula(string arrayFormula, int rowNumber, int columnNumber, 
    FormulaParseOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arrayFormula | String | Array-Formel. |
| rowNumber | Int32 | Anzahl der Zeilen, um das Ergebnis der Array-Formel zu füllen. |
| columnNumber | Int32 | Anzahl der Spalten, um das Ergebnis der Array-Formel zu füllen. |
| Optionen | FormulaParseOptions | Optionen zum Parsen der Formel. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetArrayFormulaWithStringInt32Int32FormulaParseOpDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Füge Beispieldaten in die Zellen C1:E1 ein
            cells["C1"].PutValue(10);
            cells["D1"].PutValue(20);
            cells["E1"].PutValue(30);

            // Setze eine Array-Formel in Zelle A1, die auf 2 Zeilen und 3 Spalten ausgedehnt wird
            cells["A1"].SetArrayFormula("=TRANSPOSE(C1:E1)", 2, 1, new FormulaParseOptions());

            // Formeln berechnen
            workbook.CalculateFormula();

            // Ergebnisse ausgeben
            Console.WriteLine("Array formula results:");
            for (int row = 0; row < 2; row++)
            {
                for (int col = 0; col < 3; col++)
                {
                    Cell cell = cells[row, col];
                    Console.WriteLine($"Cell {cell.Name}: {cell.Value}");
                }
            }
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

## SetArrayFormula(string, int, int, FormulaParseOptions, object[][]) {#setarrayformula_2}

Setzt eine Array-Formel für einen Zellbereich.

```csharp
public void SetArrayFormula(string arrayFormula, int rowNumber, int columnNumber, 
    FormulaParseOptions options, object[][] values)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arrayFormula | String | Array-Formel. |
| rowNumber | Int32 | Anzahl der Zeilen, um das Ergebnis der Array-Formel zu füllen. |
| columnNumber | Int32 | Anzahl der Spalten, um das Ergebnis der Array-Formel zu füllen. |
| Optionen | FormulaParseOptions | Optionen zum Parsen der Formel. |
| Werte | Object[][] | Werte für diese Zellen mit der angegebenen Array-Formel |

### Siehe auch

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


