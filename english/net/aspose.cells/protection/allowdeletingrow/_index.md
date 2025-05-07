---
title: Protection.AllowDeletingRow
second_title: Aspose.Cells for .NET API Reference
description: Protection property. Represents if the deletion of rows is allowed on a protected worksheet
type: docs
url: /net/aspose.cells/protection/allowdeletingrow/
---
## Protection.AllowDeletingRow property

Represents if the deletion of rows is allowed on a protected worksheet.

```csharp
public bool AllowDeletingRow { get; set; }
```

### Remarks

The rows containing the cells to be deleted must be unlocked when the sheet is protected, and "Select unlocked cells" option must be enabled.

### Examples

```csharp
// Called: if (protection.AllowDeletingRow) { flag |= 0x0002; }
private int Property_AllowDeletingRow(Protection protection)
        {
            int flag = 0;
            if (protection.AllowDeletingColumn) { flag |= 0x0001; }
            if (protection.AllowDeletingRow) { flag |= 0x0002; }
            if (protection.AllowEditingContent) { flag |= 0x0004; }
            if (protection.AllowEditingObject) { flag |= 0x0008; }
            if (protection.AllowEditingScenario) { flag |= 0x0010; }
            if (protection.AllowFiltering) { flag |= 0x0020; }
            if (protection.AllowFormattingCell) { flag |= 0x0040; }
            if (protection.AllowFormattingColumn) { flag |= 0x0080; }
            if (protection.AllowFormattingRow) { flag |= 0x0100; }
            if (protection.AllowInsertingColumn) { flag |= 0x0200; }
            if (protection.AllowInsertingHyperlink) { flag |= 0x0400; }
            if (protection.AllowInsertingRow) { flag |= 0x0800; }
            if (protection.AllowSelectingLockedCell) { flag |= 0x1000; }
            if (protection.AllowSelectingUnlockedCell) { flag |= 0x2000; }
            if (protection.AllowSorting) { flag |= 0x4000; }
            if (protection.AllowUsingPivotTable) { flag |= 0x8000; }
            return flag;
        }
```

### See Also

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


