---
title: "Klasse CalculationData"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.CalculationData Klasse. Stellt die erforderlichen Daten dar, die beim Berechnen einer Funktion benötigt werden, wie Funktionsname, Parameter ...usw"
type: docs
url: /de/net/aspose.cells/calculationdata/
---
## CalculationData class

Stellt die erforderlichen Daten beim Berechnen einer Funktion dar, wie Funktionsname, Parameter, ...etc.

```csharp
public class CalculationData
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [CalculatedValue](../../aspose.cells/calculationdata/calculatedvalue/) { get; set; } | Liest oder setzt den berechneten Wert für diese Funktion. |
| [Cell](../../aspose.cells/calculationdata/cell/) { get; } | Liest das Cell-Objekt, in dem sich die Funktion befindet. |
| [CellColumn](../../aspose.cells/calculationdata/cellcolumn/) { get; } | Liest den Spaltenindex der Zelle, in der sich die Funktion befindet. |
| [CellRow](../../aspose.cells/calculationdata/cellrow/) { get; } | Liest den Zeilenindex der Zelle, in der sich die Funktion befindet. |
| [FunctionName](../../aspose.cells/calculationdata/functionname/) { get; } | Liest den Funktionsnamen, der berechnet werden soll. |
| [ParamCount](../../aspose.cells/calculationdata/paramcount/) { get; } | Liest die Anzahl der Parameter |
| [Workbook](../../aspose.cells/calculationdata/workbook/) { get; } | Liest das Workbook-Objekt, in dem sich die Funktion befindet. |
| [Worksheet](../../aspose.cells/calculationdata/worksheet/) { get; } | Liest das Worksheet-Objekt, in dem sich die Funktion befindet. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [GetParamText](../../aspose.cells/calculationdata/getparamtext/)(int) | Liest den wörtlichen Text des Parameters am angegebenen Index. |
| [GetParamValue](../../aspose.cells/calculationdata/getparamvalue/)(int) | Liest das dargestellte Wertobjekt des Parameters an einem angegebenen Index. |
| [GetParamValueInArrayMode](../../aspose.cells/calculationdata/getparamvalueinarraymode/)(int, int, int) | Liest den/die Wert(e) des Parameters an einem angegebenen Index. Wenn der Parameter eine Art Ausdruck ist, der berechnet werden muss, wird er im Array-Modus berechnet. |

### Hinweise

Alle von dieser Klasse bereitgestellten Objekte dienen ausschließlich dem "Lese"-Zweck. Der Benutzer sollte während des Formelberechnungsprozesses keine Daten im Workbook ändern, da sonst unerwartete Ergebnisse oder Ausnahmen auftreten können.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassCalculationDataDemo
    {
        public static void Run()
        {
            try
            {
                // Erstelle ein einfaches Workbook und Worksheet
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];
                sheet.Name = "DemoSheet";

                // Füge einige Werte ein, die als Parameter in einer benutzerdefinierten Funktion verwendet werden
                sheet.Cells["A1"].PutValue(5);
                sheet.Cells["A2"].PutValue(10);

                // Setze eine Formel, die die benutzerdefinierte Funktion aufruft
                sheet.Cells["B1"].Formula = "=MYFUNC(A1, A2)";

                // Konfiguriere die Berechnungsoptionen, um eine benutzerdefinierte Engine zu verwenden
                CalculationOptions options = new CalculationOptions();
                options.CustomEngine = new DemoEngine();

                // Führe die Berechnung durch – die benutzerdefinierte Engine erhält eine CalculationData-Instanz
                workbook.CalculateFormula(options);

                // Gib das Ergebnis der benutzerdefinierten Funktion aus
                Console.WriteLine("Custom function result (B1): " + sheet.Cells["B1"].Value);

                // Speichere das Workbook zur Vollständigkeit
                workbook.Save("CalculationDataDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error while working with CalculationData: {ex.Message}");
            }
        }

        // Benutzerdefinierte Berechnungs-Engine, die den Zugriff auf CalculationData-Mitglieder demonstriert
        private class DemoEngine : AbstractCalculationEngine
        {
            public override void Calculate(CalculationData data)
            {
                // Stelle sicher, dass wir die erwartete benutzerdefinierte Funktion verarbeiten
                if (data.FunctionName != null &&
                    data.FunctionName.Equals("MYFUNC", StringComparison.OrdinalIgnoreCase))
                {
                    // Rufe Parameterwerte ab (sie werden als Objekte zurückgegeben)
                    object param0 = data.GetParamValue(0);
                    object param1 = data.GetParamValue(1);

                    // Konvertiere Parameter zu double für die Berechnung
                    double val0 = Convert.ToDouble(param0);
                    double val1 = Convert.ToDouble(param1);
                    double result = val0 + val1; // simple addition

                    // Weisen Sie das berechnete Ergebnis zu.
                    data.CalculatedValue = result;

                    // Demonstrieren Sie das Lesen schreibgeschützter Eigenschaften.
                    Console.WriteLine("[Engine] FunctionName : " + data.FunctionName);
                    Console.WriteLine("[Engine] ParamCount   : " + data.ParamCount);
                    Console.WriteLine("[Engine] CellRow      : " + data.CellRow);
                    Console.WriteLine("[Engine] CellColumn   : " + data.CellColumn);
                }
            }
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


