---
title: "FormulaParseOptions.CustomFunctionDefinition"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FormulaParseOptions özelliği. Özel işlevlerin ayrıştırılması için tanım"
type: docs
url: /tr/net/aspose.cells/formulaparseoptions/customfunctiondefinition/
---
## FormulaParseOptions.CustomFunctionDefinition property

Özel işlevlerin ayrıştırılması için tanım.

```csharp
public CustomFunctionDefinition CustomFunctionDefinition { get; set; }
```

### Açıklamalar

Bazı özel gereksinimler için, örneğin kullanıcının özel motorunda özel işlevi hesaplarken, bazı parametrelerin dizi modunda hesaplanması gerektiğinde, bu özelliği kullanarak formül ayrıştırılırken bu parametreleri dizi modu olarak işaretleyebilirsiniz. Aksi takdirde, kullanıcı daha sonra aynı sonucu elde etmek için bu özel işlevleri [`UpdateCustomFunctionDefinition`](../../workbook/updatecustomfunctiondefinition/) ile güncellemelidir.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaParseOptionsPropertyCustomFunctionDefinitionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Özel işlev tanımı oluştur
            CustomFunctionDefinition customFunction = new CustomFunctionDefinition();
            
            // Özel işlev ile formül ayrıştırma seçeneklerini ayarla
            FormulaParseOptions options = new FormulaParseOptions
            {
                CustomFunctionDefinition = customFunction,
                Parse = true
            };

            // Örnek veriyi ayarla
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["B1"].PutValue(20);

            // Formülde özel işlev kullan
            string formula = "=MY_CUSTOM_FUNCTION(A1, B1)";
            worksheet.Cells["C1"].SetFormula(formula, options);

            // Özel işlev işleme sürecini göstermek için çalışma kitabını hesapla
            workbook.CalculateFormula();

            // Sonucu kaydedin
            workbook.Save("CustomFunctionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [CustomFunctionDefinition](../../customfunctiondefinition/)
* class [FormulaParseOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


