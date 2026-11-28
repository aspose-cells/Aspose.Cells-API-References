---
title: "Cell.IsErrorValue"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell özelliği. Bu hücrenin değerinin bir hata olup olmadığını kontrol eder"
type: docs
url: /tr/net/aspose.cells/cell/iserrorvalue/
---
## Cell.IsErrorValue property

Bu hücrenin değerinin bir hata olup olmadığını kontrol eder.

```csharp
public bool IsErrorValue { get; }
```

### Açıklamalar

Ayrıca formül hücresine uygulanır ve hesaplanan sonucun bir hata olup olmadığını kontrol eder.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsErrorValueDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Bir hataya yol açacak bir formül ayarlayın
            Cell cell = cells["A1"];
            cell.Formula = "=1/0"; // Division by zero error
            
            // Formülleri hesapla
            workbook.CalculateFormula();

            // IsErrorValue özelliğini gösterin
            Console.WriteLine("Cell A1 value: " + cell.StringValue);
            Console.WriteLine("IsErrorValue: " + cell.IsErrorValue);
            Console.WriteLine("Error type: " + cell.Value);

            // Geçerli bir değer ayarlayın
            Cell cell2 = cells["A2"];
            cell2.PutValue("Valid value");
            
            Console.WriteLine("\nCell A2 value: " + cell2.StringValue);
            Console.WriteLine("IsErrorValue: " + cell2.IsErrorValue);

            // Bir SPILL hatası ayarla (Excel 365+ dinamik dizi formülü hatası)
            Cell cell3 = cells["A3"];
            cell3.SetDynamicArrayFormula("=A1:A10", new FormulaParseOptions(), true);
            
            Console.WriteLine("\nCell A3 value: " + cell3.StringValue);
            Console.WriteLine("IsErrorValue: " + cell3.IsErrorValue);
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


