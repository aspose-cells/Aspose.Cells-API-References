---
title: Row.IsBlank
second_title: Aspose.Cells for .NET API Reference
description: Row property. Indicates whether the row contains any data
type: docs
url: /net/aspose.cells/row/isblank/
---
## Row.IsBlank property

Indicates whether the row contains any data

```csharp
public bool IsBlank { get; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(rowSrc.IsBlank, rowDest.IsBlank, info + ".IsBlank");
public static void Property_IsBlank(Row rowSrc, Row rowDest, string info)
        {
            if (AssertHelper.checkNull(rowSrc, rowDest, info))
            {
                return;
            }
            //AssertHelper.AreEqual(rowSrc.EndHere, rowDest.EndHere, info + ".EndHere");
            AssertHelper.AreEqual(rowSrc.IsBlank, rowDest.IsBlank, info + ".IsBlank");
            AssertHelper.AreEqual(rowSrc.IsHeightMatched, rowDest.IsHeightMatched, info + ".IsHeightMatched");
            //AssertHelper.AreEqual(rowSrc.IsHidden, rowDest.IsHidden, info + ".IsHidden");
            //AssertHelper.AreEqual(rowSrc.OutlineLevel, rowDest.OutlineLevel, info + ".OutlineLevel");
            StylesTest.Check(rowSrc.GetStyle(), rowDest.GetStyle(), info + ".Style");
        }
```

### See Also

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


