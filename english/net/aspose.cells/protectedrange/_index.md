---
title: Class ProtectedRange
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.ProtectedRange class. A specified range to be allowed to edit when the sheet protection is ON
type: docs
url: /net/aspose.cells/protectedrange/
---
## ProtectedRange class

A specified range to be allowed to edit when the sheet protection is ON.

```csharp
public class ProtectedRange
```

## Properties

| Name | Description |
| --- | --- |
| [CellArea](../../aspose.cells/protectedrange/cellarea/) { get; } | Gets the [`CellArea`](./cellarea/) object represents the cell area to be protected. |
| [IsProtectedWithPassword](../../aspose.cells/protectedrange/isprotectedwithpassword/) { get; } | Indicates whether the worksheets is protected with password. |
| [Name](../../aspose.cells/protectedrange/name/) { get; set; } | Gets the Range title. This is used as a descriptor, not as a named range definition. |
| [Password](../../aspose.cells/protectedrange/password/) { get; set; } | Represents the password to protect the range. |
| [SecurityDescriptor](../../aspose.cells/protectedrange/securitydescriptor/) { get; set; } | The security descriptor defines user accounts who may edit this range without providing a password to access the range. |

## Methods

| Name | Description |
| --- | --- |
| [AddArea](../../aspose.cells/protectedrange/addarea/)(int, int, int, int) | Adds a referred area to this |
| [GetAreas](../../aspose.cells/protectedrange/getareas/)() | Gets all referred areas. |

### Examples

```csharp
// Called: ProtectedRange range = allowRanges[0];
[Test]
        //http://www.aspose.com/community/forums/thread/226241/trouble-with-allow-users-to-edit-ranges.aspx
        public void Type_ProtectedRange()
        {
            Console.WriteLine(&quot;Type_ProtectedRange()&quot;);
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

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


