---
title: Column.Index
second_title: Aspose.Cells for .NET API Reference
description: Column property. Gets the index of this column
type: docs
url: /net/aspose.cells/column/index/
---
## Column.Index property

Gets the index of this column.

```csharp
public int Index { get; }
```

### Examples

```csharp
// Called: if (columnSrc.Index == columnDest.Index)
public static void Property_Index(ColumnCollection columnsSrc, ColumnCollection columnsDest, string info)
        {
            if (AssertHelper.checkNull(columnsSrc, columnsDest, info))
            {
                return;
            }
            int srcCount = columnsSrc.Count;
            int destCount = columnsDest.Count;
            AssertHelper.AreEqual(srcCount, destCount, info + &quot;.Count&quot;);
            for (int i = 0; i &lt; srcCount ; i++)
            {
                Column columnSrc = columnsSrc[i];
                bool IsSame = false;
                for (int j = 0; j &lt; destCount; j++)
                {
                    Column columnDest = columnsDest[j];
                    IsSame = false;
                    if (columnSrc.Index == columnDest.Index)
                    {
                        Property_Index(columnSrc, columnDest, info + &quot;[&quot; + columnSrc.Index + &quot;]&quot;);
                        IsSame = true;
                        break;
                    }
                }
                if (!IsSame)
                {
                    AssertHelper.Fail(&quot;column&quot; + columnSrc.Index + &quot; isn&apos;t same!&quot;);
                }               
            }
        }
```

### See Also

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


