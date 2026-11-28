---
title: "Workbook.IsDigitallySigned"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook özelliği. Bu elektronik tablonun dijital olarak imzalı olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells/workbook/isdigitallysigned/
---
## Workbook.IsDigitallySigned property

Bu elektronik tablonun dijital olarak imzalı olup olmadığını gösterir.

```csharp
public bool IsDigitallySigned { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyIsDigitallySignedDemo
    {
        public static void Run()
        {
            // Dijital olarak imzalı bir çalışma kitabını yükle
            Workbook book = new Workbook("Test_DigiSign.xlsx");
            
            // Çalışma kitabının dijital olarak imzalı olup olmadığını kontrol et
            bool isSigned = book.IsDigitallySigned;
            Console.WriteLine("Workbook is digitally signed: " + isSigned);

            if (isSigned)
            {
                // Kopyasını kaydet (imza korunacak)
                book.Save("SignedCopy.xlsx");
                
                // Dijital imzayı kaldır
                book.RemoveDigitalSignature();
                book.Save("UnsignedCopy.xlsx");
                
                // İmzanın kaldırıldığını doğrulayın
                Workbook unsignedBook = new Workbook("UnsignedCopy.xlsx");
                Console.WriteLine("After removal, workbook is signed: " + unsignedBook.IsDigitallySigned);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


