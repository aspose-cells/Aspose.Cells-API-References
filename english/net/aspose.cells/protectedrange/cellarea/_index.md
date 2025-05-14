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
// Called: + range.CellArea.EndRow + "," + range.CellArea.EndColumn);
//http://www.aspose.com/community/forums/thread/226241/trouble-with-allow-users-to-edit-ranges.aspx
public void ProtectedRange_Property_CellArea()
{
    Console.WriteLine("ProtectedRange_Property_CellArea()");
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

* struct [CellArea](../../cellarea/)
* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


