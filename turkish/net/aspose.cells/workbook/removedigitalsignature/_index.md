---
title: "Workbook.RemoveDigitalSignature"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook yöntemi. Bu elektronik tablodan dijital imzayı kaldırır"
type: docs
url: /tr/net/aspose.cells/workbook/removedigitalsignature/
---
## Workbook.RemoveDigitalSignature method

Bu elektronik tablodan dijital imzayı kaldırır.

```csharp
public void RemoveDigitalSignature()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodRemoveDigitalSignatureDemo
    {
        public static void Run()
        {
            // Dijital imzalı bir çalışma kitabı oluşturun
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            sheet.Cells["A1"].PutValue("Test Digital Signature");
            
            // Dijital imza ile kaydedin (gerçek senaryoda bu dışarıdan imzalanır)
            string signedPath = "SignedWorkbook.xlsx";
            book.Save(signedPath, SaveFormat.Xlsx);

            // İmzalı çalışma kitabını yükleyin
            Workbook signedBook = new Workbook(signedPath);
            Console.WriteLine("Workbook is digitally signed: " + signedBook.IsDigitallySigned);

            // Dijital imzayı kaldırın
            signedBook.RemoveDigitalSignature();
            string unsignedPath = "UnsignedWorkbook.xlsx";
            signedBook.Save(unsignedPath);

            // İmzanın kaldırıldığını doğrulayın
            Workbook unsignedBook = new Workbook(unsignedPath);
            Console.WriteLine("After removal, workbook is digitally signed: " + unsignedBook.IsDigitallySigned);
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


