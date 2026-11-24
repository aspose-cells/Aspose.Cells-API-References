---
title: "Worksheet.CalculateArrayFormula"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Methode. Berechnet eine Formel als Array-Formel"
type: docs
url: /de/net/aspose.cells/worksheet/calculatearrayformula/
---
## CalculateArrayFormula(string, CalculationOptions) {#calculatearrayformula}

Berechnet eine Formel als Matrixformel.

```csharp
public object[][] CalculateArrayFormula(string formula, CalculationOptions opts)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Formel | String | Zu berechnende Formel. |
| opts | CalculationOptions | Optionen zum Berechnen der Formel |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCalculateArrayFormulaWithStringCalculationOptionsDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Einige Beispieldaten einfügen
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(5);
            worksheet.Cells["B3"].PutValue(6);

            // Eine Array-Formel definieren
            string arrayFormula = "=SUM(A1:B3)";
            
            // Berechnen Sie die Array-Formel mit Berechnungsoptionen
            object[][] result = worksheet.CalculateArrayFormula(arrayFormula, new CalculationOptions());
            
            // Gib das Ergebnis aus
            Console.WriteLine("Result of array formula calculation: " + result[0][0]);
        }
    }
}
```

### Siehe auch

* class [CalculationOptions](../../calculationoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CalculateArrayFormula(string, CalculationOptions, int, int) {#calculatearrayformula_1}

Berechnet eine Formel als Matrixformel.

```csharp
public object[][] CalculateArrayFormula(string formula, CalculationOptions opts, int maxRowCount, 
    int maxColumnCount)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Formel | String | Zu berechnende Formel. |
| opts | CalculationOptions | Optionen zum Berechnen der Formel |
| maxRowCount | Int32 | die maximale Zeilenanzahl der Ergebnisdaten. Wenn sie nicht positiv ist oder größer als die tatsächliche Zeilenanzahl, wird die tatsächliche Zeilenanzahl verwendet. |
| maxColumnCount | Int32 | die maximale Spaltenanzahl der Ergebnisdaten. Wenn sie nicht positiv ist oder größer als die tatsächliche Zeilenanzahl, wird die tatsächliche Spaltenanzahl verwendet. |

### Rückgabewert

Berechnetes Formelergebnis.

### Hinweise

Die Formel wird als dynamische Array-Formel verwendet, um die Dimension und das Ergebnis zu berechnen. Die vom Benutzer angegebene maximale Dimension wird in Fällen verwendet, in denen das berechnete Ergebnis ein großer Datensatz ist (zum Beispiel kann das berechnete Ergebnis einer gesamten Zeile oder Spalte entsprechen), der Benutzer jedoch gemäß geschäftlicher Anforderungen oder aus Leistungsgründen kein so großes Array benötigt.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCalculateArrayFormulaWithStringCalculationOptionsInt32IDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe und greifen Sie auf das erste Arbeitsblatt zu
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Beispiel 1: Einfache Berechnung einer Array-Formel
            string formula = "=ISBLANK(IF(TRUE,B2:B5))";
            CalculationOptions options = new CalculationOptions();
            object[][] result = sheet.CalculateArrayFormula(formula, options, 1, 1);
            Console.WriteLine("Result of ISBLANK(IF(TRUE,B2:B5)): " + result[0][0]);

            // Beispiel 2: Array-Formel mit dynamischem Bereich
            formula = "=LEN(IF({1;2;3;4},B2:B5))";
            result = sheet.CalculateArrayFormula(formula, options, 1, 1);
            Console.WriteLine("Result of LEN(IF({1;2;3;4},B2:B5)): " + result[0][0]);

            // Beispiel 3: Array-Formel mit MATCH-Funktion
            // Richten Sie einige Testdaten ein
            sheet.Cells["B2"].PutValue(5);
            sheet.Cells["B3"].PutValue(10);
            sheet.Cells["C2"].PutValue(1);
            sheet.Cells["C3"].PutValue(2);
            sheet.Cells["D2"].PutValue(0);
            sheet.Cells["D3"].PutValue(0);

            formula = "=MATCH(1,IF(B2:B5=5,C2:C5,D2:D5),0)";
            result = sheet.CalculateArrayFormula(formula, options, 1, 1);
            Console.WriteLine("Result of MATCH formula: " + result[0][0]);
        }
    }
}
```

### Siehe auch

* class [CalculationOptions](../../calculationoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CalculateArrayFormula(string, FormulaParseOptions, CalculationOptions, int, int, int, int, CalculationData) {#calculatearrayformula_2}

Berechnet eine Formel als Matrixformel.

```csharp
public object[][] CalculateArrayFormula(string formula, FormulaParseOptions pOpts, 
    CalculationOptions cOpts, int baseCellRow, int baseCellColumn, int maxRowCount, 
    int maxColumnCount, CalculationData calculationData)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Formel | String | Zu berechnende Formel. |
| pOpts | FormulaParseOptions | Optionen zum Parsen der Formel |
| cOpts | CalculationOptions | Optionen zum Berechnen der Formel |
| baseCellRow | Int32 | Der Zeilenindex der Basiszelle. |
| baseCellColumn | Int32 | Der Spaltenindex der Basiszelle. |
| maxRowCount | Int32 | Die maximale Zeilenanzahl der Ergebnisdaten. Wenn sie nicht positiv ist oder größer als die tatsächliche Zeilenanzahl, wird die tatsächliche Zeilenanzahl verwendet. |
| maxColumnCount | Int32 | Die maximale Spaltenanzahl der Ergebnisdaten. Wenn sie nicht positiv ist oder größer als die tatsächliche Zeilenanzahl, wird die tatsächliche Spaltenanzahl verwendet. |
| calculationData | CalculationData | Die Berechnungsdaten. Sie werden für den Fall verwendet, dass der Benutzer beim Implementieren einer benutzerdefinierten Berechnungs‑Engine einige statische Formeln berechnen muss. In einem solchen Fall muss der Benutzer sie mit den für [`Calculate`](../../abstractcalculationengine/calculate/) bereitgestellten Berechnungsdaten angeben. |

### Rückgabewert

Berechnetes Formelergebnis.

### Hinweise

Die Formel wird als dynamische Array-Formel verwendet, um die Dimension und das Ergebnis zu berechnen. Die vom Benutzer angegebene maximale Dimension wird in Fällen verwendet, in denen das berechnete Ergebnis ein großer Datensatz ist (zum Beispiel kann das berechnete Ergebnis einer gesamten Zeile oder Spalte entsprechen), der Benutzer jedoch gemäß geschäftlicher Anforderungen oder aus Leistungsgründen kein so großes Array benötigt.

### Siehe auch

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [CalculationOptions](../../calculationoptions/)
* class [CalculationData](../../calculationdata/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


