---
title: "ErrorCheckOption.GetCountOfRange"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ErrorCheckOption yöntemi. Bu ayar tarafından etkilenen aralıkların sayısını alır"
type: docs
url: /tr/net/aspose.cells/errorcheckoption/getcountofrange/
---
## ErrorCheckOption.GetCountOfRange method

Bu ayar tarafından etkilenen aralıkların sayısını alır.

```csharp
public int GetCountOfRange()
```

### Dönüş Değeri

Bu ayar tarafından etkilenen aralıkların sayısı.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ErrorCheckOptionMethodGetCountOfRangeDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Hata kontrol seçenekleri koleksiyonunu al
            ErrorCheckOptionCollection optsCollection = sheet.ErrorCheckOptions;

            // İlk hata kontrol seçeneğini ekle
            int index1 = optsCollection.Add();
            ErrorCheckOption opts1 = optsCollection[index1];
            opts1.SetErrorCheck(ErrorCheckType.NumberStoredAsText, false);
            opts1.AddRange(CellArea.CreateCellArea("A1", "D2"));
            opts1.AddRange(CellArea.CreateCellArea("A3", "D3"));

            // İkinci hata kontrol seçeneğini ekle
            int index2 = optsCollection.Add();
            ErrorCheckOption opts2 = optsCollection[index2];
            opts2.SetErrorCheck(ErrorCheckType.TwoDigitTextYear, false);
            opts2.AddRange(CellArea.CreateCellArea("A3", "D5"));

            // GetCountOfRange yöntemini göster
            Console.WriteLine("First option range count: " + opts1.GetCountOfRange());
            Console.WriteLine("Second option range count: " + opts2.GetCountOfRange());

            // Çalışma kitabını kaydedin
            workbook.Save("ErrorCheckOptionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


