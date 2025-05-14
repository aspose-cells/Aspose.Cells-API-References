---
title: ProtectedRange.Name
second_title: Aspose.Cells for .NET API Reference
description: ProtectedRange property. Gets the Range title. This is used as a descriptor not as a named range definition
type: docs
url: /net/aspose.cells/protectedrange/name/
---
## ProtectedRange.Name property

Gets the Range title. This is used as a descriptor, not as a named range definition.

```csharp
public string Name { get; set; }
```

### Examples

```csharp
// Called: Console.WriteLine(range.Name);
//http://www.aspose.com/community/forums/thread/226241/trouble-with-allow-users-to-edit-ranges.aspx
public void ProtectedRange_Property_Name()
{
    Console.WriteLine("ProtectedRange_Property_Name()");
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


