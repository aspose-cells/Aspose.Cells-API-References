---
title: Protection.AllowSelectingUnlockedCell
second_title: Aspose.Cells for .NET API Reference
description: Protection property. Represents if the user is allowed to select unlocked cells on a protected worksheet
type: docs
url: /net/aspose.cells/protection/allowselectingunlockedcell/
---
## Protection.AllowSelectingUnlockedCell property

Represents if the user is allowed to select unlocked cells on a protected worksheet.

```csharp
public bool AllowSelectingUnlockedCell { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(protectionSrc.AllowSelectingUnlockedCell, protectionDest.AllowSelectingUnlockedCell, info + ".AllowSelectingUnlockedCell");
public static void Protection_Property_AllowSelectingUnlockedCell(Protection protectionSrc, Protection protectionDest, string info)
        {
            if (AssertHelper.checkNull(protectionSrc, protectionDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(protectionSrc.AllowDeletingColumn, protectionDest.AllowDeletingColumn, info + ".AllowDeletingColumn");
            AssertHelper.AreEqual(protectionSrc.AllowDeletingRow, protectionDest.AllowDeletingRow, info + ".AllowDeletingRow");
            AssertHelper.AreEqual(protectionSrc.AllowEditingContent, protectionDest.AllowEditingContent, info + ".AllowEditingContent");
            AssertHelper.AreEqual(protectionSrc.AllowEditingObject, protectionDest.AllowEditingObject, info + ".AllowEditingObject");
            AssertHelper.AreEqual(protectionSrc.AllowEditingScenario, protectionDest.AllowEditingScenario, info + ".AllowEditingScenario");
            AssertHelper.AreEqual(protectionSrc.AllowFiltering, protectionDest.AllowFiltering, info + ".AllowFiltering");
            AssertHelper.AreEqual(protectionSrc.AllowFormattingCell, protectionDest.AllowFormattingCell, info + ".AllowFormattingCell");
            AssertHelper.AreEqual(protectionSrc.AllowFormattingColumn, protectionDest.AllowFormattingColumn, info + ".AllowFormattingColumn");
            AssertHelper.AreEqual(protectionSrc.AllowFormattingRow, protectionDest.AllowFormattingRow, info + ".AllowFormattingRow");
            AssertHelper.AreEqual(protectionSrc.AllowInsertingColumn, protectionDest.AllowInsertingColumn, info + ".AllowInsertingColumn");
            AssertHelper.AreEqual(protectionSrc.AllowInsertingHyperlink, protectionDest.AllowInsertingHyperlink, info + ".AllowInsertingHyperlink");
            AssertHelper.AreEqual(protectionSrc.AllowInsertingRow, protectionDest.AllowInsertingRow, info + ".AllowInsertingRow");
            AssertHelper.AreEqual(protectionSrc.AllowSelectingLockedCell, protectionDest.AllowSelectingLockedCell, info + ".AllowSelectingLockedCell");
            AssertHelper.AreEqual(protectionSrc.AllowSelectingUnlockedCell, protectionDest.AllowSelectingUnlockedCell, info + ".AllowSelectingUnlockedCell");
            AssertHelper.AreEqual(protectionSrc.AllowSorting, protectionDest.AllowSorting, info + ".AllowSorting");
            AssertHelper.AreEqual(protectionSrc.AllowUsingPivotTable, protectionDest.AllowUsingPivotTable, info + ".AllowUsingPivotTable");
            AssertHelper.AreEqual(protectionSrc.Password, protectionDest.Password, info + ".Password");
        }
```

### See Also

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


