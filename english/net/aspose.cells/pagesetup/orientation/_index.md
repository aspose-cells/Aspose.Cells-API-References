---
title: PageSetup.Orientation
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. Represents page print orientation
type: docs
url: /net/aspose.cells/pagesetup/orientation/
---
## PageSetup.Orientation property

Represents page print orientation.

```csharp
public PageOrientationType Orientation { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(PageOrientationType.Portrait, pageSetup.Orientation, "pageSetup.Orientation");
private void Property_Orientation(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets["Sheet1"];
            PageSetup pageSetup = sheet.PageSetup;
            AssertHelper.AreEqual(PageOrientationType.Portrait, pageSetup.Orientation, "pageSetup.Orientation");
        }
```

### See Also

* enum [PageOrientationType](../../pageorientationtype/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


