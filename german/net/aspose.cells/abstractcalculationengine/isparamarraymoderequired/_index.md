---
title: "AbstractCalculationEngine.IsParamArrayModeRequired"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AbstractCalculationEngine‑Eigenschaft. Gibt an, ob dieser Engine den Parameter im Array‑Modus berechnen muss. Der Standardwert ist false. Wenn GetParamValueInArrayMode beim Berechnen benutzerdefinierter Funktionen erforderlich ist und der Benutzer die Definition dafür nicht mit UpdateCustomFunctionDefinition aktualisiert hat, muss diese Eigenschaft auf true gesetzt werden."
type: docs
url: /de/net/aspose.cells/abstractcalculationengine/isparamarraymoderequired/
---
## AbstractCalculationEngine.IsParamArrayModeRequired property

Gibt an, ob dieser Engine den Parameter im Array‑Modus berechnet werden muss. Der Standardwert ist false. Wenn [`GetParamValueInArrayMode`](../../calculationdata/getparamvalueinarraymode/) beim Berechnen benutzerdefinierter Funktionen erforderlich ist und der Benutzer die Definition dafür nicht (mit [`UpdateCustomFunctionDefinition`](../../workbook/updatecustomfunctiondefinition/)) aktualisiert hat, muss diese Eigenschaft auf true gesetzt werden.

```csharp
public virtual bool IsParamArrayModeRequired { get; }
```

### Hinweise

Wenn dieser benutzerdefinierte Berechnungs‑Engine den Parameter im Array‑Modus berechnen muss, werden weitere Stacks benötigt, um den Baum für die Parameter zu puffern, und die Methode Calculate() kann rekursiv aufgerufen werden, um den Parameterwert zu berechnen. Aus Leistungsgründen sollten Sie diese Eigenschaft bei fehlenden speziellen Anforderungen beim Standardwert (false) belassen.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractCalculationEnginePropertyIsParamArrayModeRequiredDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            CustomCalculationEngine engine = new CustomCalculationEngine();
            Console.WriteLine("IsParamArrayModeRequired: " + engine.IsParamArrayModeRequired);

            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].Formula = "=SUMARRAY(A1,A2)";

            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = engine;
            workbook.CalculateFormula(options);

            Console.WriteLine("SUMARRAY result: " + worksheet.Cells["A3"].Value);

            workbook.Save("IsParamArrayModeRequiredDemo.xlsx");
        }
    }

    public class CustomCalculationEngine : AbstractCalculationEngine
    {
        public override bool IsParamArrayModeRequired => true;

        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "SUMARRAY")
            {
                double sum = 0;
                for (int i = 0; i < data.ParamCount; i++)
                {
                    Aspose.Cells.ReferredArea paramArea1 = (Aspose.Cells.ReferredArea)data.GetParamValue(i);

                    double param1 = Convert.ToDouble(paramArea1.GetValue(0, 0));

                    sum += param1;
                }
                data.CalculatedValue = sum;
            }
        }

        public override bool ForceRecalculate(string functionName)
        {
            return false;
        }
    }
}
```

### Siehe auch

* class [AbstractCalculationEngine](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


