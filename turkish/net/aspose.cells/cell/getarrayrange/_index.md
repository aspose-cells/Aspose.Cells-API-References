---
title: "Cell.GetArrayRange"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell yöntemi. Hücre formülü bir dizi formülü ise dizi aralığını alır"
type: docs
url: /tr/net/aspose.cells/cell/getarrayrange/
---
## Cell.GetArrayRange method

Hücrenin formülü bir dizi formülü ise dizi aralığını alır.

```csharp
public CellArea GetArrayRange()
```

### Dönüş Değeri

Dizi aralığı.

### Açıklamalar

Yalnızca hücrenin formülü bir dizi formülü olduğunda uygulanır

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetArrayRangeDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // A1 hücresine dinamik dizi formülü ayarla.
            Cell cell = cells[0, 0];
            string formula = "=SEQUENCE(3,2)";
            cell.SetDynamicArrayFormula(formula, new FormulaParseOptions(), false);
            
            // Formülleri hesapla
            wb.CalculateFormula();
            
            // Dinamik formülün dizi aralığını al
            CellArea arrayRange = cell.GetArrayRange();
            
            // Dizi aralığı bilgilerini çıktı olarak ver
            Console.WriteLine("Array range for dynamic formula:");
            Console.WriteLine($"Start row: {arrayRange.StartRow}");
            Console.WriteLine($"Start column: {arrayRange.StartColumn}");
            Console.WriteLine($"End row: {arrayRange.EndRow}");
            Console.WriteLine($"End column: {arrayRange.EndColumn}");
            
            // Dizi aralığındaki değerleri yazdır
            Console.WriteLine("\nValues in the array range:");
            for (int r = arrayRange.StartRow; r <= arrayRange.EndRow; r++)
            {
                for (int c = arrayRange.StartColumn; c <= arrayRange.EndColumn; c++)
                {
                    Console.Write(cells[r, c].Value + "\t");
                }
                Console.WriteLine();
            }
        }
    }
}
```

### Ayrıca Bakınız

* struct [CellArea](../../cellarea/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


