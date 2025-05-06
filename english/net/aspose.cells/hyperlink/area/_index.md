---
title: Hyperlink.Area
second_title: Aspose.Cells for .NET API Reference
description: Hyperlink property. Gets the range of hyperlink
type: docs
url: /net/aspose.cells/hyperlink/area/
---
## Hyperlink.Area property

Gets the range of hyperlink.

```csharp
public CellArea Area { get; }
```

### Examples

```csharp
// Called: if (linkSrc.Area.StartRow == linkDest.Area.StartRow &amp;amp;&amp;amp; linkSrc.Area.StartColumn == linkDest.Area.StartColumn
public static void Property_Area(HyperlinkCollection hlinksSrc, HyperlinkCollection hlinksDest, string info)
        {
            if (AssertHelper.checkNull(hlinksSrc, hlinksDest, info))
            {
                return;
            }
            int countSrc = hlinksSrc.Count;
            int countDest = hlinksDest.Count;
            AssertHelper.AreEqual(countSrc, countDest, info + &quot;.Count&quot;);
            bool IsSame = false;
            for (int i = 0; i &lt; countSrc; i++)
            {
                Hyperlink linkSrc = hlinksSrc[i];                
                for (int j = 0; j &lt; countDest; j++)
                {
                    IsSame = false;
                    Hyperlink linkDest = hlinksDest[j];
                    if (linkSrc.Area.StartRow == linkDest.Area.StartRow &amp;&amp; linkSrc.Area.StartColumn == linkDest.Area.StartColumn
                        &amp;&amp; linkSrc.Area.EndRow == linkDest.Area.EndRow &amp;&amp; linkSrc.Area.EndColumn == linkDest.Area.EndColumn)
                    {
                        IsSame = true;
                        Property_Area(linkSrc, linkDest, info);
                        break;
                    }
                }
                if (!IsSame)
                {
                    AssertHelper.Fail(&quot;Hyperlinks object isn&apos;t same!&quot;);
                }
            }
        }
```

### See Also

* struct [CellArea](../../cellarea/)
* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


