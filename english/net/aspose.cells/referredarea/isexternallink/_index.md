---
title: ReferredArea.IsExternalLink
second_title: Aspose.Cells for .NET API Reference
description: ReferredArea property. Indicates whether this is an external link
type: docs
url: /net/aspose.cells/referredarea/isexternallink/
---
## ReferredArea.IsExternalLink property

Indicates whether this is an external link.

```csharp
public bool IsExternalLink { get; }
```

### Examples

```csharp
// Called: if (ra.IsExternalLink)
public object ReferredArea_Property_IsExternalLink(object dest)
            {
                ReferredArea ra = (ReferredArea)dest;
                StringBuilder sb = new StringBuilder();
                if (ra.IsExternalLink)
                {
                    sb.Append('[');
                    sb.Append(ra.ExternalFileName);
                    sb.Append(']');
                }
                sb.Append(ra.SheetName).Append('!').Append(CellsHelper.CellIndexToName(ra.StartRow, ra.StartColumn));
                if (ra.IsArea)
                {
                    sb.Append(':').Append(CellsHelper.CellIndexToName(ra.EndRow, ra.EndColumn));
                }
                return sb.ToString();
            }
```

### See Also

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


