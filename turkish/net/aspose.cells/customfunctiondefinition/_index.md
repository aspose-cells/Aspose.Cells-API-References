---
title: "Sınıf CustomFunctionDefinition"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.CustomFunctionDefinition sınıfı. Kullanıcıların özel motoru ile hesaplama yapan özel fonksiyonun tanımı"
type: docs
url: /tr/net/aspose.cells/customfunctiondefinition/
---
## CustomFunctionDefinition class

Kullanıcının özel motoru ile hesaplama yapan özel işlevin tanımı.

```csharp
public class CustomFunctionDefinition
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [CustomFunctionDefinition](customfunctiondefinition/)() | Varsayılan yapıcı. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| virtual [GetArrayModeParameters](../../aspose.cells/customfunctiondefinition/getarraymodeparameters/)(string) | Verilen özel fonksiyonun dizi modunda hesaplanması gereken parametre indekslerini alır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomFunctionDefinitionDemo
    {
        public static void CustomFunctionDefinitionExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Yeni bir CustomFunctionDefinition örneği oluştur
            CustomFunctionDefinition customFunctionDefinition = new CustomFunctionDefinition();

            // Yeni bir FormulaParseOptions örneği oluştur ve CustomFunctionDefinition'ı ayarla
            FormulaParseOptions formulaParseOptions = new FormulaParseOptions
            {
                CustomFunctionDefinition = customFunctionDefinition
            };

            // Çalışma kitabına bir çalışma sayfası ekle
            Worksheet worksheet = workbook.Worksheets[0];

            // Özel bir formül tanımla
            string customFormula = "=MY_CUSTOM_FUNCTION(A1, B1)";

            // FormulaParseOptions kullanarak özel formülü ayrıştır
            worksheet.Cells["C1"].Formula = customFormula;
            worksheet.Cells["C1"].SetFormula(customFormula, formulaParseOptions);

            // Çalışma kitabını kaydedin
            workbook.Save("CustomFunctionDefinitionExample.xlsx");
            workbook.Save("CustomFunctionDefinitionExample.pdf");
            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


