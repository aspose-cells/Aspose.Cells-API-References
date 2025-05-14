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
// Called: range.Password = "1";
//http://www.aspose.com/community/forums/thread/226241/trouble-with-allow-users-to-edit-ranges.aspx
public void ProtectedRange_Property_Password()
{
    Console.WriteLine("ProtectedRange_Property_Password()");
    string infn = path + "Test_AllowEditRanges.xlsm";
    string outfn = Constants.destPath + "Test_AllowEditRanges_out.xlsm";

    Workbook book = new Workbook(infn);
    Worksheet sheet = book.Worksheets[0];
    ProtectedRangeCollection allowRanges = sheet.AllowEditRanges;
    ProtectedRange range = allowRanges[0];
    Console.WriteLine(range.Name);
    Console.Write("  " + range.CellArea.StartRow + "," + range.CellArea.StartColumn + ","
      + range.CellArea.EndRow + "," + range.CellArea.EndColumn);
    Console.WriteLine("  " + range.Password);
    //Console.WriteLine("  " + range.SecurityDescriptor);

    int idx = allowRanges.Add("r2", 1, 1, 3, 3);
    range = allowRanges[idx];
    range.Password = "1";

    book.Save(outfn);
}
```

### See Also

* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


