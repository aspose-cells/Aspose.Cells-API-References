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
// Called: equals(columnSrc, columnDest, info + "[" + columnSrc.Index + "]");
public static void Property_Index(ColumnCollection columnsSrc, ColumnCollection columnsDest, string info)
        {
            if (AssertHelper.checkNull(columnsSrc, columnsDest, info))
            {
                return;
            }
            int srcCount = columnsSrc.Count;
            int destCount = columnsDest.Count;
            AssertHelper.AreEqual(srcCount, destCount, info + ".Count");
            for (int i = 0; i < srcCount ; i++)
            {
                Column columnSrc = columnsSrc[i];
                bool IsSame = false;
                for (int j = 0; j < destCount; j++)
                {
                    Column columnDest = columnsDest[j];
                    IsSame = false;
                    if (columnSrc.Index == columnDest.Index)
                    {
                        Property_Index(columnSrc, columnDest, info + "[" + columnSrc.Index + "]");
                        IsSame = true;
                        break;
                    }
                }
                if (!IsSame)
                {
                    AssertHelper.Fail("column" + columnSrc.Index + " isn't same!");
                }               
            }
        }
```

### See Also

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


