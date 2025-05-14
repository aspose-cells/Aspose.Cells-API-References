---
title: PasteOptions.PasteType
second_title: Aspose.Cells for .NET API Reference
description: PasteOptions property. The paste special type
type: docs
url: /net/aspose.cells/pasteoptions/pastetype/
---
## PasteOptions.PasteType property

The paste special type.

```csharp
public PasteType PasteType { get; set; }
```

### Examples

```csharp
// Called: targetRange.Copy(sourceRange, new PasteOptions() { PasteType = PasteType.All });
public void PasteOptions_Property_PasteType()
{
    Workbook workbook = new Workbook();
    Worksheet worksheet = workbook.Worksheets[0];

    Cell cell = worksheet.Cells["A1"];
    cell.PutValue("1");

    Aspose.Cells.Range sourceRange = worksheet.Cells.CreateRange("A1");
    Aspose.Cells.Range targetRange = worksheet.Cells.CreateRange("B1:B3");

    targetRange.Copy(sourceRange, new PasteOptions() { PasteType = PasteType.All });

    Assert.AreEqual(worksheet.Cells["A1"].StringValue, "1");
    Assert.AreEqual(worksheet.Cells["B1"].StringValue, "1");
    Assert.AreEqual(worksheet.Cells["B2"].StringValue, "1");
    Assert.AreEqual(worksheet.Cells["B3"].StringValue, "1");
}
```

### See Also

* enum [PasteType](../../pastetype/)
* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


