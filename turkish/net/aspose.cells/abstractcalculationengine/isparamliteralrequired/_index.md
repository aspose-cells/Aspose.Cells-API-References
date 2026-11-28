---
title: "AbstractCalculationEngine.IsParamLiteralRequired"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AbstractCalculationEngine özelliği. Bu motorun bir hesaplama yaparken parametrenin gerçek metin değerine ihtiyacı olup olmadığını gösterir. Varsayılan değer false'tur."
type: docs
url: /tr/net/aspose.cells/abstractcalculationengine/isparamliteralrequired/
---
## AbstractCalculationEngine.IsParamLiteralRequired property

Bu motorun bir hesaplama yaparken parametrenin gerçek metnini gerekip gerektirmediğini gösterir. Varsayılan değer false'tur.

```csharp
public virtual bool IsParamLiteralRequired { get; }
```

### Açıklamalar

Bu özel hesaplama motoru parametrenin gerçek metin değerine ihtiyaç duyuyorsa, parametreler için gerçek metni önbelleğe almak üzere daha fazla yığın (stack) gerekecek ve `Calculate()` yöntemi parametrenin değerini hesaplamak için yinelemeli (recursive) olarak çağrılabilir. Genel olarak formüllerin hesaplanması için gerçek metin gerekli değildir ve bu özelliğin çoğu uygulama için daha iyi performans elde etmek amacıyla false olarak bırakılması önerilir.

### Örnekler

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

            // Özel hesaplama motoru örneği oluştur
            MyCustomEngine engine = new MyCustomEngine();

            // Mevcut özellik değerini oku
            Console.WriteLine("Current IsParamLiteralRequired value: " + engine.IsParamLiteralRequired);

            // Dize literal parametresiyle test formülü oluştur
            worksheet.Cells["A1"].Formula = "=MYFUNC(\"123\")";

            // Özel hesaplama seçenekleriyle çalışma kitabını hesapla
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = engine;
            workbook.CalculateFormula(options);

            // Özellik değerine göre hesaplama sonucunu göster
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

### Ayrıca Bakınız

* class [AbstractCalculationEngine](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


