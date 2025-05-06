---
title: Protection.AllowInsertingRow
second_title: Aspose.Cells for .NET API Reference
description: Protection property. Represents if the insertion of rows is allowed on a protected worksheet
type: docs
url: /net/aspose.cells/protection/allowinsertingrow/
---
## Protection.AllowInsertingRow property

Represents if the insertion of rows is allowed on a protected worksheet

```csharp
public bool AllowInsertingRow { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(protectionSrc.AllowInsertingRow, protectionDest.AllowInsertingRow, info + &amp;quot;.AllowInsertingRow&amp;quot;);
public static void Property_AllowInsertingRow(Protection protectionSrc, Protection protectionDest, string info)
        {
            if (AssertHelper.checkNull(protectionSrc, protectionDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(protectionSrc.AllowDeletingColumn, protectionDest.AllowDeletingColumn, info + &quot;.AllowDeletingColumn&quot;);
            AssertHelper.AreEqual(protectionSrc.AllowDeletingRow, protectionDest.AllowDeletingRow, info + &quot;.AllowDeletingRow&quot;);
            AssertHelper.AreEqual(protectionSrc.AllowEditingContent, protectionDest.AllowEditingContent, info + &quot;.AllowEditingContent&quot;);
            AssertHelper.AreEqual(protectionSrc.AllowEditingObject, protectionDest.AllowEditingObject, info + &quot;.AllowEditingObject&quot;);
            AssertHelper.AreEqual(protectionSrc.AllowEditingScenario, protectionDest.AllowEditingScenario, info + &quot;.AllowEditingScenario&quot;);
            AssertHelper.AreEqual(protectionSrc.AllowFiltering, protectionDest.AllowFiltering, info + &quot;.AllowFiltering&quot;);
            AssertHelper.AreEqual(protectionSrc.AllowFormattingCell, protectionDest.AllowFormattingCell, info + &quot;.AllowFormattingCell&quot;);
            AssertHelper.AreEqual(protectionSrc.AllowFormattingColumn, protectionDest.AllowFormattingColumn, info + &quot;.AllowFormattingColumn&quot;);
            AssertHelper.AreEqual(protectionSrc.AllowFormattingRow, protectionDest.AllowFormattingRow, info + &quot;.AllowFormattingRow&quot;);
            AssertHelper.AreEqual(protectionSrc.AllowInsertingColumn, protectionDest.AllowInsertingColumn, info + &quot;.AllowInsertingColumn&quot;);
            AssertHelper.AreEqual(protectionSrc.AllowInsertingHyperlink, protectionDest.AllowInsertingHyperlink, info + &quot;.AllowInsertingHyperlink&quot;);
            AssertHelper.AreEqual(protectionSrc.AllowInsertingRow, protectionDest.AllowInsertingRow, info + &quot;.AllowInsertingRow&quot;);
            AssertHelper.AreEqual(protectionSrc.AllowSelectingLockedCell, protectionDest.AllowSelectingLockedCell, info + &quot;.AllowSelectingLockedCell&quot;);
            AssertHelper.AreEqual(protectionSrc.AllowSelectingUnlockedCell, protectionDest.AllowSelectingUnlockedCell, info + &quot;.AllowSelectingUnlockedCell&quot;);
            AssertHelper.AreEqual(protectionSrc.AllowSorting, protectionDest.AllowSorting, info + &quot;.AllowSorting&quot;);
            AssertHelper.AreEqual(protectionSrc.AllowUsingPivotTable, protectionDest.AllowUsingPivotTable, info + &quot;.AllowUsingPivotTable&quot;);
            AssertHelper.AreEqual(protectionSrc.Password, protectionDest.Password, info + &quot;.Password&quot;);
        }
```

### See Also

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


