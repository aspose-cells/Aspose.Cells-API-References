---
title: "AbstractCalculationEngine.IsParamLiteralRequired"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AbstractCalculationEngine-Eigenschaft. Gibt an, ob diese Engine den wörtlichen Text des Parameters während einer Berechnung benötigt. Standardwert ist false"
type: docs
url: /de/net/aspose.cells/abstractcalculationengine/isparamliteralrequired/
---
## AbstractCalculationEngine.IsParamLiteralRequired property

Gibt an, ob diese Engine den wörtlichen Text des Parameters während einer Berechnung benötigt. Der Standardwert ist false.

```csharp
public virtual bool IsParamLiteralRequired { get; }
```

### Hinweise

Wenn diese benutzerdefinierte Berechnungs-Engine den wörtlichen Text des Parameters benötigt, sind zusätzliche Stacks erforderlich, um den wörtlichen Text der Parameter zu zwischenspeichern, und die Calculate()-Methode kann rekursiv aufgerufen werden, um den Wert des Parameters zu berechnen. In der Regel wird der wörtliche Text für die Berechnung von Formeln nicht benötigt, und diese Eigenschaft sollte für die meisten Implementierungen auf false belassen werden, um eine bessere Leistung zu erzielen.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractCalculationEnginePropertyIsParamLiteralRequiredDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle eine Instanz einer benutzerdefinierten Berechnungs-Engine
            MyCustomEngine engine = new MyCustomEngine();

            // Lese den aktuellen Eigenschaftswert
            Console.WriteLine("Current IsParamLiteralRequired value: " + engine.IsParamLiteralRequired);

            // Erstelle eine Testformel mit einem Zeichenketten-Literal-Parameter
            worksheet.Cells["A1"].Formula = "=MYFUNC(\"123\")";

            // Berechne die Arbeitsmappe mit benutzerdefinierten Berechnungsoptionen
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = engine;
            workbook.CalculateFormula(options);

            // Zeige das Berechnungsergebnis basierend auf dem Eigenschaftswert an
            Console.WriteLine("Formula result: " + worksheet.Cells["A1"].StringValue);

            workbook.Save("IsParamLiteralRequiredDemo.xlsx");
        }
    }

    public class MyCustomEngine : AbstractCalculationEngine
    {
        public override bool IsParamLiteralRequired => true;

        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName.Equals("MYFUNC", StringComparison.OrdinalIgnoreCase))
            {
                if (data.ParamCount > 0)
                {                    
                    object paramValue = data.GetParamValue(0);
                    string result = (paramValue is string) ? "Literal received" : "Value received";
                    data.CalculatedValue = result;
                }
            }
        }
    }
}
```

### Siehe auch

* class [AbstractCalculationEngine](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


