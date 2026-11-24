---
title: "Klasse AbstractCalculationEngine"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.AbstractCalculationEngine Klasse. Stellt die benutzerdefinierte Berechnungs‑Engine des Benutzers dar, um die Standard‑Berechnungs‑Engine von Aspose.Cells zu erweitern."
type: docs
url: /de/net/aspose.cells/abstractcalculationengine/
---
## AbstractCalculationEngine class

Stellt die benutzerdefinierte Berechnungs-Engine des Benutzers dar, um die Standard-Berechnungs-Engine von Aspose.Cells zu erweitern.

```csharp
public abstract class AbstractCalculationEngine
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| virtual [IsParamArrayModeRequired](../../aspose.cells/abstractcalculationengine/isparamarraymoderequired/) { get; } | Gibt an, ob diese Engine den Parameter im Array‑Modus berechnen muss. Der Standardwert ist false. Wenn [`GetParamValueInArrayMode`](../calculationdata/getparamvalueinarraymode/) beim Berechnen benutzerdefinierter Funktionen erforderlich ist und der Benutzer die Definition dafür nicht aktualisiert hat (mit [`UpdateCustomFunctionDefinition`](../workbook/updatecustomfunctiondefinition/)), muss diese Eigenschaft auf true gesetzt werden. |
| virtual [IsParamLiteralRequired](../../aspose.cells/abstractcalculationengine/isparamliteralrequired/) { get; } | Gibt an, ob diese Engine den wörtlichen Text des Parameters während einer Berechnung benötigt. Der Standardwert ist false. |
| virtual [ProcessBuiltInFunctions](../../aspose.cells/abstractcalculationengine/processbuiltinfunctions/) { get; } | Ob integrierte Funktionen, die von der integrierten Engine unterstützt werden, von dieser Implementierung geprüft und verarbeitet werden sollen. Der Standardwert ist false. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| abstract [Calculate](../../aspose.cells/abstractcalculationengine/calculate/)(CalculationData) | Berechnet eine Funktion mit den angegebenen Daten. |
| virtual [ForceRecalculate](../../aspose.cells/abstractcalculationengine/forcerecalculate/)(string) | Ob die gegebene Funktion beim Berechnen gemeinsamer Formeln immer neu berechnet werden soll. |
| [SkipCalculation](../../aspose.cells/abstractcalculationengine/skipcalculation/)() | Überspringt die Berechnung der gesamten Formel, die die derzeit ausgewertete Funktion referenziert. |

### Hinweise

Der Benutzer sollte keinen Teil des Arbeitsbuchs direkt in dieser Implementierung ändern (außer dem berechneten Ergebnis der benutzerdefinierten Funktion, das über die Eigenschaft CalculationData.CalculatedValue festgelegt werden kann). Andernfalls können unerwartete Ergebnisse oder Ausnahmen auftreten. Wenn der Benutzer andere Daten als das berechnete Ergebnis in der Implementierung für einige benutzerdefinierte Funktionen ändern muss, zum Beispiel die Formel einer Zelle, den Stil usw., sollte er diese Daten in dieser Implementierung sammeln und außerhalb des Formel‑Berechnungs‑Kontexts ändern.

### Beispiele

```csharp
using Aspose.Cells;
using System;

namespace AsposeCellsExamples
{
    public class CustomCalculationEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            // Beispiel: Benutzerdefinierte Implementierung für eine Funktion mit dem Namen \"MYFUNC\"
            if (data.FunctionName.ToUpper() == "MYFUNC")
            {
                // Angenommen, MYFUNC nimmt zwei Parameter entgegen und gibt deren Summe zurück
                Aspose.Cells.ReferredArea paramArea1 = (Aspose.Cells.ReferredArea)data.GetParamValue(0);
                Aspose.Cells.ReferredArea paramArea2 = (Aspose.Cells.ReferredArea)data.GetParamValue(1);

                double param1 = Convert.ToDouble(paramArea1.GetValue(0, 0));
                double param2 = Convert.ToDouble(paramArea2.GetValue(0, 0));
                data.CalculatedValue = param1 + param2;
            }
        }

        public override bool ForceRecalculate(string functionName)
        {
            // Erzwinge die Neuberechnung für die benutzerdefinierte Funktion \"MYFUNC\"
            return functionName.ToUpper() == "MYFUNC";
        }
    }

    public class CalculationEngineDemo
    {
        public static void Test()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Werte in Zellen einfügen
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);

            // Fügen Sie eine Formel hinzu, die die benutzerdefinierte Funktion verwendet
            sheet.Cells["A3"].Formula = "=MYFUNC(A1, A2)";

            // Berechnungsoptionen mit der benutzerdefinierten Engine festlegen
            CalculationOptions options = new CalculationOptions
            {
                CustomEngine = new CustomCalculationEngine(),
                IgnoreError = false,
                Recursive = true
            };

            // Formeln mit der benutzerdefinierten Engine berechnen
            workbook.CalculateFormula(options);

            // Geben Sie das Ergebnis der benutzerdefinierten Funktion aus
            Console.WriteLine("Result of MYFUNC(A1, A2): " + sheet.Cells["A3"].Value);

            // Speichere die Arbeitsmappe
            workbook.Save("CustomCalculationEngineExample.xlsx");
            workbook.Save("CustomCalculationEngineExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


