---
title: "Cell.GetFormula"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell yöntemi. Bu hücrenin formülünü al"
type: docs
url: /tr/net/aspose.cells/cell/getformula/
---
## Cell.GetFormula method

Bu hücrenin formülünü al.

```csharp
public string GetFormula(bool isR1C1, bool isLocal)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| isR1C1 | Boolean | Formülün R1C1 olarak biçimlendirilmesi gerekip gerekmediği. |
| isLocal | Boolean | Formülün yerel ayarlara göre biçimlendirilmesi gerekip gerekmediği. |

### Dönüş Değeri

bu hücrenin formülü.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetFormulaWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ve formüller ekle
            Cell cellA1 = worksheet.Cells["A1"];
            cellA1.PutValue(10);
            
            Cell cellB1 = worksheet.Cells["B1"];
            cellB1.PutValue(20);
            
            Cell cellC1 = worksheet.Cells["C1"];
            cellC1.Formula = "=A1+B1";
            
            // GetFormula'ı farklı parametrelerle göster
            Console.WriteLine("Standard formula: " + cellC1.GetFormula(false, false));
            Console.WriteLine("Local formula: " + cellC1.GetFormula(false, true));
            
            // Formül stilini yerel olarak değiştir ve farkı göster
            workbook.Settings.CultureInfo = new System.Globalization.CultureInfo("de-DE");
            Console.WriteLine("Local formula after culture change: " + cellC1.GetFormula(false, true));
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


