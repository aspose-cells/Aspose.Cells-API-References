---
title: "FormatCondition.SetFormulas"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FormatCondition yöntemi. Bu biçim koşuluyla ilişkili değeri veya ifadeyi ayarlar"
type: docs
url: /tr/net/aspose.cells/formatcondition/setformulas/
---
## FormatCondition.SetFormulas method

Bu biçim koşuluyla ilişkili değeri veya ifadeyi ayarlar.

```csharp
public void SetFormulas(string formula1, string formula2, bool isR1C1, bool isLocal)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| formula1 | String | Bu biçim koşuluyla ilişkili değer veya ifade. Girdi değeri '=' ile başlıyorsa, formül olarak kabul edilir. Aksi takdirde düz değer (metin, sayı, bool) olarak kabul edilir. '=' ile başlayan metin değeri için kullanıcı, formülü şu formatta girebilir: "=\"=...\"". |
| formula2 | String | Bu biçim koşuluyla ilişkili değer veya ifade. Giriş biçimi formula1 ile aynı |
| isR1C1 | Boolean | Formülün R1C1 formülü olup olmadığı. |
| isLocal | Boolean | Formülün yerel biçimlendirilip biçimlendirilmediği. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionMethodSetFormulasWithStringStringBooleanBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            ConditionalFormattingCollection cfs = worksheet.ConditionalFormattings;
            int formatIndex = cfs.Add();
            FormatConditionCollection fcs = cfs[formatIndex];
            
            fcs.AddArea(CellArea.CreateCellArea("A1", "C10"));
            
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue);
            FormatCondition fc = fcs[conditionIndex];
            
            fc.Operator = OperatorType.Between;
            fc.SetFormulas("=1", "=2", false, false);
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


