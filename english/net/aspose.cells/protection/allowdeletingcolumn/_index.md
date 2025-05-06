---
title: Protection.AllowDeletingColumn
second_title: Aspose.Cells for .NET API Reference
description: Protection property. Represents if the deletion of columns is allowed on a protected worksheet
type: docs
url: /net/aspose.cells/protection/allowdeletingcolumn/
---
## Protection.AllowDeletingColumn property

Represents if the deletion of columns is allowed on a protected worksheet.

```csharp
public bool AllowDeletingColumn { get; set; }
```

### Remarks

The columns containing the cells to be deleted must be unlocked when the sheet is protected, and "Select unlocked cells" option must be enabled.

### Examples

```csharp
// Called: protection.AllowDeletingColumn = (flag &amp;amp; 0x01) != 0;
private void Property_AllowDeletingColumn(Protection protection, int flag)
        {
            protection.AllowDeletingColumn = (flag &amp; 0x01) != 0;
            protection.AllowDeletingRow = (flag &amp; 0x02) != 0;
            protection.AllowEditingContent = (flag &amp; 0x04) != 0;
            protection.AllowEditingObject = (flag &amp; 0x08) != 0;
            protection.AllowEditingScenario = (flag &amp; 0x10) != 0;
            protection.AllowFiltering = (flag &amp; 0x20) != 0;
            protection.AllowFormattingCell = (flag &amp; 0x40) != 0;
            protection.AllowFormattingColumn = (flag &amp; 0x80) != 0;
            protection.AllowFormattingRow = (flag &amp; 0x0100) != 0;
            protection.AllowInsertingColumn = (flag &amp; 0x0200) != 0;
            protection.AllowInsertingHyperlink = (flag &amp; 0x0400) != 0;
            protection.AllowInsertingRow = (flag &amp; 0x0800) != 0;
            protection.AllowSelectingLockedCell = (flag &amp; 0x1000) != 0;
            protection.AllowSelectingUnlockedCell = (flag &amp; 0x2000) != 0;
            protection.AllowSorting = (flag &amp; 0x4000) != 0;
            protection.AllowUsingPivotTable = (flag &amp; 0x8000) != 0;
        }
```

### See Also

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


