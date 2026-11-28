---
title: "CalculationData.GetParamValue"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CalculationData yöntemi. Belirli bir indeksdeki parametrenin temsil edilen değer nesnesini alır"
type: docs
url: /tr/net/aspose.cells/calculationdata/getparamvalue/
---
## CalculationData.GetParamValue method

Verilen indeksdeki parametrenin temsil edilen değer nesnesini alır.

```csharp
public object GetParamValue(int index)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| indeks | Int32 | Parametrenin indeksi (0 tabanlı) |

### Dönüş Değeri

Parametrenin hesaplanmış değeri.

### Açıklamalar

Tek bir parametre için:

Eğer düz bir değer ise, doğrudan o değeri döndürür;

Eğer bir referans ise, ReferredArea nesnesini döndürür;

Eğer birden çok değere sahip veri kümesine referans veriyorsa, nesneler dizisini döndürür;

Eğer hesaplanması gereken bir ifade türü ise, değer modunda hesaplanır ve genellikle mevcut hücre temeline göre tek bir değer döndürülür. Örneğin, D2 formülünün bir parametresi A:A+B:B ise, A2+B2 hesaplanıp döndürülür. Ancak, bu parametre dizi modu olarak belirtilmişse (by [`UpdateCustomFunctionDefinition`](../../workbook/updatecustomfunctiondefinition/) veya [`CustomFunctionDefinition`](../../formulaparseoptions/customfunctiondefinition/) tarafından), öğeleri A1+B1,A2+B2,... olan bir dizi (object[][]) döndürülür.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationDataMethodGetParamValueWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].Formula = "=HYPERLINK(\"http://localhost:9090\", \"Target\")";

            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = new HyperlinkCalculationEngine();
            workbook.CalculateFormula(options);
        }

        class HyperlinkCalculationEngine : AbstractCalculationEngine
        {
            public override void Calculate(CalculationData data)
            {
                if (data.FunctionName.Equals("HYPERLINK", StringComparison.OrdinalIgnoreCase))
                {
                    Console.WriteLine("URL Parameter: " + data.GetParamValue(0));
                    Console.WriteLine("Display Text: " + data.GetParamValue(1));
                }
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


