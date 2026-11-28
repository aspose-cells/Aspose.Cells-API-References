---
title: "CalculationOptions.CustomEngine"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CalculationOptions özelliği. Aspose.Cells'in varsayılan hesaplama motorunu genişletmek için özel formül hesaplama motoru"
type: docs
url: /tr/net/aspose.cells/calculationoptions/customengine/
---
## CalculationOptions.CustomEngine property

Aspose.Cells'in varsayılan hesaplama motorunu genişletmek için özel formül hesaplama motoru.

```csharp
public AbstractCalculationEngine CustomEngine { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationOptionsPropertyCustomEngineDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // A1 hücresine HYPERLINK formülünü ayarlayın
            sheet.Cells["A1"].Formula = "=HYPERLINK(\"http://example.com\",\"Click Here\")";
            
            // HYPERLINK işlevini işleyen özel bir motor oluşturun
            CustomEngineForHyperlink customEngine = new CustomEngineForHyperlink(true);
            
            // Özel motor ile hesaplama seçeneklerini ayarlayın
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = customEngine;
            
            // Formülleri özel motor ile hesaplayın
            wb.CalculateFormula(options);
            
            Console.WriteLine("Custom engine invoked: " + customEngine.Invoked);
        }
    }

    public class CustomEngineForHyperlink : AbstractCalculationEngine
    {
        public bool Invoked { get; private set; }
        private readonly bool _shouldProcess;

        public CustomEngineForHyperlink(bool shouldProcess)
        {
            _shouldProcess = shouldProcess;
        }

        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "HYPERLINK" && _shouldProcess)
            {
                Invoked = true;
                data.CalculatedValue = "[Custom Processed] " + data.GetParamText(1);
            }
            // Base.Calculate() metodunu çağırmayın çünkü soyut.
            // Diğer işlevler için varsayılan hesaplamanın gerçekleşmesine izin verin.
        }
    }
}
```

### Ayrıca Bakınız

* class [AbstractCalculationEngine](../../abstractcalculationengine/)
* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


