---
title: "AbstractCalculationEngine.ForceRecalculate"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AbstractCalculationEngine yöntemi. Paylaşılan formüller hesaplanırken verilen fonksiyonun her zaman yeniden hesaplanmasını zorunlu kılıp kılmayacağını belirler"
type: docs
url: /tr/net/aspose.cells/abstractcalculationengine/forcerecalculate/
---
## AbstractCalculationEngine.ForceRecalculate method

Paylaşılan formüller hesaplanırken verilen fonksiyonun her zaman yeniden hesaplanmasını zorlayıp zorlamayacağı.

```csharp
public virtual bool ForceRecalculate(string functionName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| functionName | String | fonksiyonun adı. Genellikle bu, özel fonksiyonun adıdır. Eğer [`ProcessBuiltInFunctions`](../processbuiltinfunctions/) doğru ise, yerleşik fonksiyonlar da burada kontrol edilir. |

### Dönüş Değeri

belirtilen fonksiyonun her zaman yeniden hesaplanması gerekiyorsa doğru.

### Açıklamalar

Paylaşılan formüller için, birden fazla hücre aynı fonksiyonu paylaşır. Fonksiyonun parametreleri bu hücreler için de aynı kalırsa, genellikle bu fonksiyon yalnızca bir kez hesaplanmalıdır. Bu nedenle performans açısından bu tür fonksiyonları yalnızca bir kez hesaplarız ([`Calculate`](../calculate/) sadece bir kez çağrılır, her hücre için tekrar tekrar çağrılmak yerine). Ancak, kullanıcının özel uygulamasında, özellikle özel fonksiyonların, farklı hücreler için farklı şekilde hesaplanması gerekebilir. Bu durumda, kullanıcı bu yöntemi geçersiz kılarak fonksiyon için true döndürmelidir. Ve [`Calculate`](../calculate/) için, verilen [`CalculatedValue`](../../calculationdata/calculatedvalue/) önceki hesaplamanın önbelleğe alınmış değeriyle başlatılmış olabilir.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;


    public class AbstractCalculationEngineMethodForceRecalculateWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            MyCustomEngine engine = new MyCustomEngine();
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = engine;

            worksheet.Cells["A1"].Formula = "MYVOLATILEFUNC()";

            try
            {
                bool result = engine.ForceRecalculate("MYVOLATILEFUNC");
                Console.WriteLine($"ForceRecalculate returned: {result} for 'MYVOLATILEFUNC'");

                workbook.CalculateFormula(options);
                Console.WriteLine($"First calculation result: {worksheet.Cells["A1"].Value}");

                System.Threading.Thread.Sleep(1000);
                workbook.CalculateFormula(options);
                Console.WriteLine($"Second calculation result: {worksheet.Cells["A1"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ForceRecalculate: {ex.Message}");
            }

            workbook.Save("ForceRecalculateDemo.xlsx");
        }
    }


    public class MyCustomEngine : AbstractCalculationEngine
    {
        private int calculationCount = 0;

        public override bool ForceRecalculate(string functionName)
        {
            return functionName == "MYVOLATILEFUNC";
        }

        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "MYVOLATILEFUNC")
            {
                calculationCount++;
                data.CalculatedValue = calculationCount;
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [AbstractCalculationEngine](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


