---
title: "ErrorCheckOption.AddRange"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ErrorCheckOption yöntemi. Bu ayar tarafından bir etkilenen aralık ekler"
type: docs
url: /tr/net/aspose.cells/errorcheckoption/addrange/
---
## ErrorCheckOption.AddRange method

Bu ayar tarafından etkilenen bir aralık ekler.

```csharp
public int AddRange(CellArea ca)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ca | CellArea | eklenecek aralık. |

### Dönüş Değeri

bu ayarın aralık listesinde eklenen aralığın indeksi.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ErrorCheckOptionMethodAddRangeWithCellAreaDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            ErrorCheckOptionCollection optsCollection = sheet.ErrorCheckOptions;
            int index = optsCollection.Add();
            ErrorCheckOption opts = optsCollection[index];
            
            opts.SetErrorCheck(ErrorCheckType.NumberStoredAsText, false);
            
            // CellArea kullanarak aralıklar ekle
            opts.AddRange(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 1, EndColumn = 3 }); // A1:D2
            opts.AddRange(new CellArea { StartRow = 2, StartColumn = 0, EndRow = 2, EndColumn = 3 }); // A3:D3
            
            // Çalışma kitabını kaydedin
            workbook.Save("ErrorCheckOptionMethodAddRangeWithCellAreaDemo.xls");
            
            Console.WriteLine("Workbook saved with error check options.");
        }
    }
}
```

### Ayrıca Bakınız

* struct [CellArea](../../cellarea/)
* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


