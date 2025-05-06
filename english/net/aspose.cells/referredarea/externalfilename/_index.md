---
title: ReferredArea.ExternalFileName
second_title: Aspose.Cells for .NET API Reference
description: ReferredArea property. Get the external file name if this is an external reference
type: docs
url: /net/aspose.cells/referredarea/externalfilename/
---
## ReferredArea.ExternalFileName property

Get the external file name if this is an external reference.

```csharp
public string ExternalFileName { get; }
```

### Examples

```csharp
// Called: sb.Append(ra.ExternalFileName);
public object Property_ExternalFileName(object dest)
            {
                ReferredArea ra = (ReferredArea)dest;
                StringBuilder sb = new StringBuilder();
                if (ra.IsExternalLink)
                {
                    sb.Append(&apos;[&apos;);
                    sb.Append(ra.ExternalFileName);
                    sb.Append(&apos;]&apos;);
                }
                sb.Append(ra.SheetName).Append(&apos;!&apos;).Append(CellsHelper.CellIndexToName(ra.StartRow, ra.StartColumn));
                if (ra.IsArea)
                {
                    sb.Append(&apos;:&apos;).Append(CellsHelper.CellIndexToName(ra.EndRow, ra.EndColumn));
                }
                return sb.ToString();
            }
```

### See Also

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


