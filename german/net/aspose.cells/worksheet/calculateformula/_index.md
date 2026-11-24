---
title: "Worksheet.CalculateFormula"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Methode. Berechnet eine Formel"
type: docs
url: /de/net/aspose.cells/worksheet/calculateformula/
---
## CalculateFormula(string) {#calculateformula}

Berechnet eine Formel.

```csharp
public object CalculateFormula(string formula)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Formel | String | Zu berechnende Formel. |

### Rückgabewert

Berechnetes Formelergebnis.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCalculateFormulaWithStringDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            wb.Settings.Region = CountryCode.USA;
            Worksheet sheet = wb.Worksheets[0];

            // Grundlegende Zahlenumwandlung demonstrieren
            string formula = "=NUMBERVALUE(\"1.234\")";
            Console.WriteLine("NUMBERVALUE(\"1.234\") = " + sheet.CalculateFormula(formula));

            // Währungsumwandlung demonstrieren
            formula = "=NUMBERVALUE(\"$1,234.56\")";
            Console.WriteLine("NUMBERVALUE(\"$1,234.56\") = " + sheet.CalculateFormula(formula));

            // Zeitumwandlung demonstrieren
            formula = "=NUMBERVALUE(\"0:25\")";
            Console.WriteLine("NUMBERVALUE(\"0:25\") = " + sheet.CalculateFormula(formula));

            // Datumsumwandlung demonstrieren
            formula = "=NUMBERVALUE(\"07/26/2023\")";
            Console.WriteLine("NUMBERVALUE(\"07/26/2023\") = " + sheet.CalculateFormula(formula));

            // Fehlerfall demonstrieren
            formula = "=NUMBERVALUE(\"invalid\")";
            Console.WriteLine("NUMBERVALUE(\"invalid\") = " + sheet.CalculateFormula(formula));
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CalculateFormula(string, CalculationOptions) {#calculateformula_1}

Berechnet einen Formelausdruck direkt.

```csharp
public object CalculateFormula(string formula, CalculationOptions opts)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Formel | String | Zu berechnende Formel. |
| opts | CalculationOptions | Optionen zum Berechnen der Formel |

### Rückgabewert

Berechnetes Ergebnis der angegebenen Formel. Das zurückgegebene Objekt kann mögliche Typen von [`Value`](../../cell/value/) oder ReferredArea haben.

### Hinweise

Die Formel wird genau so berechnet, wie sie in Zelle A1 festgelegt wurde. Und die Formel wird als normale Formel behandelt. Wenn Sie die Formel als Array‑Formel berechnen und ein Array für das berechnete Ergebnis erhalten möchten, verwenden Sie stattdessen [`CalculateArrayFormula`](../calculatearrayformula/).

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCalculateFormulaWithStringCalculationOptionsDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Einige Beispieldaten einfügen
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            
            // Erstellen Sie eine benutzerdefinierte Berechnungs-Engine
            CustomEngine customEngine = new CustomEngine();
            
            // Formel mit benutzerdefinierter Engine berechnen
            CalculationOptions options = new CalculationOptions
            {
                CustomEngine = customEngine
            };
            
            object result = worksheet.CalculateFormula("=SUM(A1:A3)", options);
            
            Console.WriteLine("Calculation result: " + result);
        }
    }

    public class CustomEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "SUM")
            {
                double sum = 0;
                for (int i = 0; i < data.ParamCount; i++)
                {
                    object value = data.GetParamValue(i);
                    if (value is double)
                    {
                        sum += (double)value;
                    }
                }
                data.CalculatedValue = sum;
            }
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

## CalculateFormula(string, FormulaParseOptions, CalculationOptions, int, int, CalculationData) {#calculateformula_2}

Berechnet einen Formelausdruck direkt.

```csharp
public object CalculateFormula(string formula, FormulaParseOptions pOpts, CalculationOptions cOpts, 
    int baseCellRow, int baseCellColumn, CalculationData calculationData)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Formel | String | Zu berechnende Formel. |
| pOpts | FormulaParseOptions | Optionen zum Parsen der Formel. |
| cOpts | CalculationOptions | Optionen zum Berechnen der Formel. |
| baseCellRow | Int32 | Der Zeilenindex der Basiszelle. |
| baseCellColumn | Int32 | Der Spaltenindex der Basiszelle. |
| calculationData | CalculationData | Die Berechnungsdaten. Sie werden für den Fall verwendet, dass der Benutzer beim Implementieren einer benutzerdefinierten Berechnungs‑Engine einige statische Formeln berechnen muss. In einem solchen Fall muss der Benutzer sie mit den für [`Calculate`](../../abstractcalculationengine/calculate/) bereitgestellten Berechnungsdaten angeben. |

### Rückgabewert

Berechnetes Ergebnis der angegebenen Formel. Das zurückgegebene Objekt kann mögliche Typen von [`Value`](../../cell/value/) oder ReferredArea haben.

### Hinweise

Die Formel wird genau so berechnet, wie sie in der angegebenen Basiszelle festgelegt wurde. Und die Formel wird als normale Formel behandelt. Wenn Sie die Formel als Array‑Formel berechnen und ein Array für das berechnete Ergebnis erhalten möchten, verwenden Sie stattdessen [`CalculateArrayFormula`](../calculatearrayformula/).

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCalculateFormulaWithStringFormulaParseOptCalculati169472Demo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten befüllen
            worksheet.Cells["B1"].PutValue(5);
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["C1"].PutValue(2);
            worksheet.Cells["C2"].PutValue(4);

            // Berechnungsoptionen definieren
            CalculationOptions calculationOptions = new CalculationOptions();
            
            // Formel‑Parse‑Optionen definieren
            FormulaParseOptions formulaParseOptions = new FormulaParseOptions();
            
            // Formel mit allen Parametern berechnen
            object result = worksheet.CalculateFormula(
                "=SUM(B1:B2, C1:C2)",  // formula
                formulaParseOptions,   // parse options
                calculationOptions,    // calculation options
                0,                     // base cell row
                0,                     // base cell column
                null                   // calculation data
            );

            // Gib das Ergebnis aus
            Console.WriteLine("Calculation result: " + result);
        }
    }
}
```

### Siehe auch

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [CalculationOptions](../../calculationoptions/)
* class [CalculationData](../../calculationdata/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CalculateFormula(CalculationOptions, bool) {#calculateformula_3}

Berechnet alle Formeln in diesem Arbeitsblatt.

```csharp
public void CalculateFormula(CalculationOptions options, bool recursive)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Optionen | CalculationOptions | Optionen für die Berechnung |
| rekursiv | Boolean | True bedeutet, wenn die Zellen des Arbeitsblatts von den Zellen anderer Arbeitsblätter abhängen, werden die abhängigen Zellen in den anderen Arbeitsblättern ebenfalls berechnet. False bedeutet, dass alle Formeln im Arbeitsblatt berechnet wurden und die Werte korrekt sind. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCalculateFormulaWithCalculationOptionsBooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten und Formeln festlegen
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["B1"].PutValue("=SUM(A1:A3)");
            
            // Berechnungsoptionen erstellen
            CalculationOptions options = new CalculationOptions();
            options.Recursive = true;
            options.IgnoreError = false;
            
            // Formel mit Optionen berechnen und vollständige Berechnung erzwingen
            worksheet.CalculateFormula(options, true);
            
            // Das berechnete Ergebnis ausgeben
            Console.WriteLine("Calculated value: " + worksheet.Cells["B1"].StringValue);
        }
    }
}
```

### Siehe auch

* class [CalculationOptions](../../calculationoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


