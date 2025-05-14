---
title: Workbook.IsDigitallySigned
second_title: Aspose.Cells for .NET API Reference
description: Workbook property. Indicates if this spreadsheet is digitally signed
type: docs
url: /net/aspose.cells/workbook/isdigitallysigned/
---
## Workbook.IsDigitallySigned property

Indicates if this spreadsheet is digitally signed.

```csharp
public bool IsDigitallySigned { get; }
```

### Examples

```csharp
// Called: bool bOutF2 = book.IsDigitallySigned;
// http://www.aspose.com/community/forums/thread/255140.aspx
public void Workbook_Property_IsDigitallySigned()
{
    Console.WriteLine("Workbook_Property_IsDigitallySigned()");
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
        throw new Exception("Workbook_Property_IsDigitallySigned() failed!");
}
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


