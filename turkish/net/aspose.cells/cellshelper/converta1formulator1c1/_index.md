---
title: "CellsHelper.ConvertA1FormulaToR1C1"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CellsHelper yöntemi. Hücrenin A1 formülünü r1c1 formülüne dönüştürür"
type: docs
url: /tr/net/aspose.cells/cellshelper/converta1formulator1c1/
---
## CellsHelper.ConvertA1FormulaToR1C1 method

Hücrenin A1 formülünü r1c1 formülüne dönüştürür.

```csharp
[Obsolete("Use Worksheet.ConvertFormulaReferenceStyle() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public static string ConvertA1FormulaToR1C1(string formula, int row, int column)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| formül | String | A1 formülü. |
| satır | Int32 | Hücrenin satır indeksi. |
| sütun | Int32 | Hücrenin sütun indeksi. |

### Dönüş Değeri

R1C1 formülü.

### Açıklamalar

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen Worksheet.ConvertFormulaReferenceStyle() yöntemini kullanın. Bu özellik, Ağustos 2023'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodConvertA1FormulaToR1C1WithStringInt32Int32Demo
    {
        public static void Run()
        {
            // A1 stilindeki formülü R1C1 stiline dönüştür
            string r1c1Formula = CellsHelper.ConvertA1FormulaToR1C1("=A1+B2", 0, 0);
            Console.WriteLine("R1C1 Formula: " + r1c1Formula);
        }
    }
}
```

### Ayrıca Bakınız

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


