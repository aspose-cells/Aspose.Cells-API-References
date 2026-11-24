---
title: "Klasse CalculationOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.CalculationOptions-Klasse. Stellt Optionen für Berechnungen dar"
type: docs
url: /de/net/aspose.cells/calculationoptions/
---
## CalculationOptions class

Stellt Optionen für die Berechnung dar.

```csharp
public class CalculationOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [CalculationOptions](calculationoptions/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [CalcStackSize](../../aspose.cells/calculationoptions/calcstacksize/) { get; set; } | Die Stapelgröße für die rekursive Berechnung von Zellen. Der Standardwert ist 200. |
| [CalculationMonitor](../../aspose.cells/calculationoptions/calculationmonitor/) { get; set; } | Der Monitor, mit dem der Benutzer den Fortschritt der Formelberechnung verfolgen kann. |
| [CharacterEncoding](../../aspose.cells/calculationoptions/characterencoding/) { get; set; } | Gibt die beim Berechnen von Formeln zu verwendende Kodierung für das Codieren/Dekodieren von Zeichen an. Für Funktionen wie CHAR, CODE hängt das berechnete Ergebnis von den Regionseinstellungen und dem Standard‑Zeichensatz der Umgebung ab. Mit dieser Eigenschaft kann der Benutzer die geeignete Kodierung für diese Funktionen festlegen, um das erwartete Ergebnis zu erhalten. |
| [CustomEngine](../../aspose.cells/calculationoptions/customengine/) { get; set; } | Die benutzerdefinierte Formelberechnungs‑Engine, um die Standard‑Berechnungs‑Engine von Aspose.Cells zu erweitern. |
| [IgnoreError](../../aspose.cells/calculationoptions/ignoreerror/) { get; set; } | Gibt an, ob beim Berechnen von Formeln auftretende Fehler ignoriert werden sollen. Der Fehler kann eine nicht unterstützte Funktion, externe Verknüpfungen usw. sein. Der Standardwert ist true. |
| [LinkedDataSources](../../aspose.cells/calculationoptions/linkeddatasources/) { get; set; } | Gibt die Datenquellen für in Formeln verwendete externe Verknüpfungen an. |
| [PrecisionStrategy](../../aspose.cells/calculationoptions/precisionstrategy/) { get; set; } | Gibt die Strategie zur Verarbeitung der Berechnungsgenauigkeit an. |
| [Recursive](../../aspose.cells/calculationoptions/recursive/) { get; set; } | Gibt an, ob abhängige Zellen rekursiv berechnet werden sollen, wenn eine Zelle berechnet wird und von anderen Zellen abhängt. Der Standardwert ist true. |
| [RefreshDynamicArrayFormula](../../aspose.cells/calculationoptions/refreshdynamicarrayformula/) { get; set; } | Gibt an, ob dynamische Array‑Formeln vor der Berechnung von Formeln aktualisiert werden sollen. |
| [UserSpecifiedRefreshDynamicArrayFormula](../../aspose.cells/calculationoptions/userspecifiedrefreshdynamicarrayformula/) { get; } | Gibt an, ob der Benutzer das Verhalten zum Aktualisieren dynamischer Array‑Formeln vor der Berechnung bestimmter Formeln explizit festgelegt hat. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Text;

    public class CalculationOptionsDemo
    {
        public static void CalculationOptionsExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue(10.555);
            worksheet.Cells["A2"].PutValue(20.6666);
            worksheet.Cells["A3"].PutValue(30.7777);
            worksheet.Cells["A4"].Formula = "=SUM(A1:A3)";

            // Erstellen Sie eine Instanz von CalculationOptions
            CalculationOptions calcOptions = new CalculationOptions
            {
                IgnoreError = true,
                Recursive = true,
                CalcStackSize = 200,
                PrecisionStrategy = CalculationPrecisionStrategy.Round,
                CharacterEncoding = Encoding.UTF8
            };

            // Optional können Sie eine benutzerdefinierte Berechnungs‑Engine oder einen Monitor festlegen.
            // calcOptions.CustomEngine = new MyCustomEngine();
            // calcOptions.CalculationMonitor = new MyCalculationMonitor();

            // Berechnen Sie Formeln in der Arbeitsmappe mit den angegebenen Optionen.
            workbook.CalculateFormula(calcOptions);

            // Speichere die Arbeitsmappe
            workbook.Save("CalculationOptionsExample.xlsx");
            workbook.Save("CalculationOptionsExample.pdf");

        }
    }

    // Beispiel für eine benutzerdefinierte Berechnungs‑Engine (falls erforderlich)
    public class MyCustomEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            // Benutzerdefinierte Berechnungslogik
            string funcName = data.FunctionName.ToUpper();
            if (funcName == "MYFUNC")
            {
                // Beispiel für benutzerdefinierte Funktionslogik
                int count = data.ParamCount;
                object result = null;
                for (int i = 0; i < count; i++)
                {
                    object paramValue = data.GetParamValue(i);
                    if (paramValue is ReferredArea)
                    {
                        ReferredArea ra = (ReferredArea)paramValue;
                        paramValue = ra.GetValue(0, 0);
                    }
                    // Verarbeiten Sie hier den Parameter
                    // result = ...;
                }
                data.CalculatedValue = result;
            }
        }
    }

    // Beispiel für benutzerdefinierten Berechnungsmonitor (falls erforderlich)
    public class MyCalculationMonitor : AbstractCalculationMonitor
    {
        public override void BeforeCalculate(int sheetIndex, int rowIndex, int colIndex)
        {
            // Logik vor der Berechnung
            Console.WriteLine($"Before calculating cell at Sheet {sheetIndex}, Row {rowIndex}, Column {colIndex}");
        }

        public override void AfterCalculate(int sheetIndex, int rowIndex, int colIndex)
        {
            // Logik nach der Berechnung
            Console.WriteLine($"After calculating cell at Sheet {sheetIndex}, Row {rowIndex}, Column {colIndex}");
        }

        public override bool OnCircular(System.Collections.IEnumerator circularCellsData)
        {
            // Zirkuläre Referenzen verarbeiten
            Console.WriteLine("Circular reference detected.");
            return true; // Continue calculation
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


