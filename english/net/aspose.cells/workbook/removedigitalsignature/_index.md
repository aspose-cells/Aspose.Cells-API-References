---
title: Workbook.RemoveDigitalSignature
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Removes digital signature from this spreadsheet
type: docs
url: /net/aspose.cells/workbook/removedigitalsignature/
---
## Workbook.RemoveDigitalSignature method

Removes digital signature from this spreadsheet.

```csharp
public void RemoveDigitalSignature()
```

### Examples

```csharp
// Called: book.RemoveDigitalSignature();
[Test]
        // http://www.aspose.com/community/forums/thread/255140.aspx
        public void Method_RemoveDigitalSignature()
        {
            Console.WriteLine("Method_RemoveDigitalSignature()");
            string infn = path + "Test_DigiSign.xlsx";
            string outfn1 = Constants.destPath + "Test_DigiSign_out_keep.xlsx";
            string outfn2 = Constants.destPath + "Test_DigiSign_out_removed.xlsx";

            Workbook book = new Workbook(infn);
            bool bInF = book.IsDigitallySigned;
            book.Save(outfn1);

            book = new Workbook(outfn1);
            bool bOutF1 = book.IsDigitallySigned;
            book.RemoveDigitalSignature();
            book.Save(outfn2);

            book = new Workbook(outfn2);
            bool bOutF2 = book.IsDigitallySigned;

            if (!bInF || !bOutF1 || bOutF2)
                throw new Exception("Method_RemoveDigitalSignature() failed!");
        }
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


