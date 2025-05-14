---
title: FormatConditionCollection.RangeCount
second_title: Aspose.Cells for .NET API Reference
description: FormatConditionCollection property. Gets count of conditionally formatted ranges
type: docs
url: /net/aspose.cells/formatconditioncollection/rangecount/
---
## FormatConditionCollection.RangeCount property

Gets count of conditionally formatted ranges.

```csharp
public int RangeCount { get; }
```

### Examples

```csharp
// Called: if (fcc.RangeCount < 1)
private void FormatConditionCollection_Property_RangeCount(ConditionalFormattingCollection cfc, string msgHeader)
        {
            foreach (FormatConditionCollection fcc in cfc)
            {
                if (fcc.RangeCount < 1)
                {
                    StringBuilder sb = new StringBuilder();
                    sb.Append(msgHeader);
                    sb.Append(" the applied range should not be empty: ");
                    GetInfo(fcc, sb);
                    Assert.Fail(sb.ToString());
                }
            }
        }
```

### See Also

* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


