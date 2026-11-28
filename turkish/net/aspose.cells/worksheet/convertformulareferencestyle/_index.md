---
title: "Worksheet.ConvertFormulaReferenceStyle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet yöntemi. Formül referans stilini dönüştürür"
type: docs
url: /tr/net/aspose.cells/worksheet/convertformulareferencestyle/
---
## Worksheet.ConvertFormulaReferenceStyle method

Formül referans stilini dönüştürür.

```csharp
public string ConvertFormulaReferenceStyle(string formula, bool toR1C1, int baseCellRow, 
    int baseCellColumn)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| formül | String | Dönüştürülecek formül. |
| toR1C1 | Boolean | Formülün dönüştürüleceği referans stili. Orijinal formül A1 referans stilindeyse, bu değer true olmalıdır, böylece formül A1'den R1C1 referans stiline dönüştürülür; Orijinal formül R1C1 referans stilindeyse, bu değer false olmalıdır, böylece formül R1C1'den A1 referans stiline dönüştürülür; |
| baseCellRow | Int32 | Temel hücrenin satır indeksi. |
| baseCellColumn | Int32 | Temel hücrenin sütun indeksi. |

### Dönüş Değeri

Dönüştürülmüş formül.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodConvertFormulaReferenceStyleWithStringBooleanInt32Int32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // Örnek 1: R1C1 stilini A1 stiline dönüştür
            string formulaR1C1 = "R[0]C23,testDS,R[0]C24";
            string formulaA1 = sheet.ConvertFormulaReferenceStyle(formulaR1C1, false, 0, 0);
            Console.WriteLine("Converted formula: " + formulaA1);

            // Örnek 2: Karışık referanslarla dönüştür
            string formulaMixed = "R[0]C23,testDS,rcurr,R[0]C24";
            string convertedMixed = sheet.ConvertFormulaReferenceStyle(formulaMixed, false, 0, 0);
            Console.WriteLine("Converted mixed formula: " + convertedMixed);
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


