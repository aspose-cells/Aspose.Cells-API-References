---
title: ProtectedRange.Password
second_title: Aspose.Cells for .NET API Reference
description: ProtectedRange property. Represents the password to protect the range
type: docs
url: /net/aspose.cells/protectedrange/password/
---
## ProtectedRange.Password property

Represents the password to protect the range.

```csharp
public string Password { get; set; }
```

### Examples

```csharp
// Called: range.Password = &amp;quot;1&amp;quot;;
[Test]
        //http://www.aspose.com/community/forums/thread/226241/trouble-with-allow-users-to-edit-ranges.aspx
        public void Property_Password()
        {
            Console.WriteLine(&quot;Property_Password()&quot;);
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

* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


