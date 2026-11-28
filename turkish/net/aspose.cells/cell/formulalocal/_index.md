---
title: "Cell.FormulaLocal"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell özelliği. Hücrenin yerel formatlı formülünü al"
type: docs
url: /tr/net/aspose.cells/cell/formulalocal/
---
## Cell.FormulaLocal property

Hücrenin yerel biçimlendirilmiş formülünü al.

```csharp
public string FormulaLocal { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyFormulaLocalDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Demonstrasyon için varsayılan yereli Almanca olarak ayarla
            workbook.Settings.Region = CountryCode.Germany;
            
            // A1 hücresine eriş
            Cell cell = worksheet.Cells["A1"];
            
            // Formülü standart formatta (İngilizce) ayarla
            cell.Formula = "=SUM(B1:C1)";
            
            // Formülleri hem standart hem de yerel formatlarda göster
            Console.WriteLine("Standard Formula: " + cell.Formula);
            Console.WriteLine("Localized Formula: " + cell.FormulaLocal);
            
            // Formülü yerel formatta (Almanca) ayarla
            cell.FormulaLocal = "=SUMME(B1:C1)";
            
            // Farkı göstermek için formülleri tekrar göster
            Console.WriteLine("\nAfter setting FormulaLocal:");
            Console.WriteLine("Standard Formula: " + cell.Formula);
            Console.WriteLine("Localized Formula: " + cell.FormulaLocal);
            
            // Yerelleştirme ile GetFormula'yu göster
            Console.WriteLine("\nUsing GetFormula:");
            Console.WriteLine("English formula: " + cell.GetFormula(false, false));
            Console.WriteLine("Localized formula: " + cell.GetFormula(false, true));
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


