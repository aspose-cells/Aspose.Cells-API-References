---
title: ProtectedRange.CellArea
second_title: Aspose.Cells for .NET API Reference
description: ProtectedRange property. Gets the CellArea object represents the cell area to be protected
type: docs
url: /net/aspose.cells/protectedrange/cellarea/
---
## ProtectedRange.CellArea property

Gets the `CellArea` object represents the cell area to be protected.

```csharp
public CellArea CellArea { get; }
```

### Examples

```csharp
// Called: + range.CellArea.EndRow + &amp;quot;,&amp;quot; + range.CellArea.EndColumn);
[Test]
        //http://www.aspose.com/community/forums/thread/226241/trouble-with-allow-users-to-edit-ranges.aspx
        public void Property_CellArea()
        {
            Console.WriteLine(&quot;Property_CellArea()&quot;);
            string infn = path + &quot;Test_AllowEditRanges.xlsm&quot;;
            string outfn = Constants.destPath + &quot;Test_AllowEditRanges_out.xlsm&quot;;

            Workbook book = new Workbook(infn);
            Worksheet sheet = book.Worksheets[0];
            ProtectedRangeCollection allowRanges = sheet.AllowEditRanges;
            ProtectedRange range = allowRanges[0];
            Console.WriteLine(range.Name);
            Console.Write(&quot;  &quot; + range.CellArea.StartRow + &quot;,&quot; + range.CellArea.StartColumn + &quot;,&quot;
              + range.CellArea.EndRow + &quot;,&quot; + range.CellArea.EndColumn);
            Console.WriteLine(&quot;  &quot; + range.Password);
            //Console.WriteLine(&quot;  &quot; + range.SecurityDescriptor);

            int idx = allowRanges.Add(&quot;r2&quot;, 1, 1, 3, 3);
            range = allowRanges[idx];
            range.Password = &quot;1&quot;;

            book.Save(outfn);
        }
```

### See Also

* struct [CellArea](../../cellarea/)
* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


