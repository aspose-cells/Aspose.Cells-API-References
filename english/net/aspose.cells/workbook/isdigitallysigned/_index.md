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
// Called: Console.WriteLine("is out file signed: " + book.IsDigitallySigned);
[Test]
        //http://www.aspose.com/community/forums/thread/224760.aspx  
        public void Property_IsDigitallySigned()
        {
            Console.WriteLine("Property_IsDigitallySigned()");
            string infn = path + "Test_IsDigitallySigned.xlsx";
            string outfn = Constants.destPath + "Test_IsDigitallySigned_out.xlsx";

            Workbook book = new Workbook(infn);
            Console.WriteLine("is src file signed: " + book.IsDigitallySigned);
            book.Save(outfn);
            book = new Workbook(outfn);
            Console.WriteLine("is out file signed: " + book.IsDigitallySigned);
        }
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


