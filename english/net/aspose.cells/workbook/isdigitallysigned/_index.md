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
// Called: Console.WriteLine(&amp;quot;is out file signed: &amp;quot; + book.IsDigitallySigned);
[Test]
        //http://www.aspose.com/community/forums/thread/224760.aspx  
        public void Property_IsDigitallySigned()
        {
            Console.WriteLine(&quot;Property_IsDigitallySigned()&quot;);
            string infn = path + &quot;Test_IsDigitallySigned.xlsx&quot;;
            string outfn = Constants.destPath + &quot;Test_IsDigitallySigned_out.xlsx&quot;;

            Workbook book = new Workbook(infn);
            Console.WriteLine(&quot;is src file signed: &quot; + book.IsDigitallySigned);
            book.Save(outfn);
            book = new Workbook(outfn);
            Console.WriteLine(&quot;is out file signed: &quot; + book.IsDigitallySigned);
        }
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


