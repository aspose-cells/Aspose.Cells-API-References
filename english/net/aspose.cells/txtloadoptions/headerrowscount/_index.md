---
title: TxtLoadOptions.HeaderRowsCount
second_title: Aspose.Cells for .NET API Reference
description: TxtLoadOptions property. The count of header rows to be repeated for extended sheets
type: docs
url: /net/aspose.cells/txtloadoptions/headerrowscount/
---
## TxtLoadOptions.HeaderRowsCount property

The count of header rows to be repeated for extended sheets.

```csharp
public int HeaderRowsCount { get; set; }
```

### Remarks

The header rows specified by this property will be duplicated for those extended sheets. This property only takes effect when [`ExtendToNextSheet`](../extendtonextsheet/) is true.

### Examples

```csharp
// Called: HeaderRowsCount = 2,
[Test]
        public void Property_HeaderRowsCount()
        {
            char[] cs = new char[450];
            for (int i = 0; i &lt; cs.Length; i += 2)
            {
                cs[i] = i % 50 == 0 ? &apos;\n&apos; : &apos;,&apos;;
                cs[i + 1] = (char)(&apos;a&apos; + ((i &gt;&gt; 1) % 26));
            }
            string content = new string(cs, 1, cs.Length - 1);
            TxtLoadOptions opts = new TxtLoadOptions()
            {
                Encoding = Encoding.Unicode,
                ExtendToNextSheet = true,
                HeaderRowsCount = 2,
                HeaderColumnsCount = 3,
                MaxRowCount = 6,
                MaxColumnCount = 8
            };
            MemoryStream ms = new MemoryStream(Encoding.Unicode.GetBytes(content), false);
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells.ImportCSV(ms, opts, 65532, 252);
        }
```

### See Also

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


