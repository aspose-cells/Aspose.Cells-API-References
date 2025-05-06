---
title: ErrorCheckOption.AddRange
second_title: Aspose.Cells for .NET API Reference
description: ErrorCheckOption method. Adds one influenced range by this setting
type: docs
url: /net/aspose.cells/errorcheckoption/addrange/
---
## ErrorCheckOption.AddRange method

Adds one influenced range by this setting.

```csharp
public int AddRange(CellArea ca)
```

| Parameter | Type | Description |
| --- | --- | --- |
| ca | CellArea | the range to be added. |

### Return Value

the index of the added range in the range list of this setting.

### Examples

```csharp
// Called: opts.AddRange(CreateCellArea(&amp;quot;A3&amp;quot;, &amp;quot;D3&amp;quot;));
[Test]
        public void Method_CellArea_()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            ErrorCheckOptionCollection optss = sheet.ErrorCheckOptions;
            int index = optss.Add();
            ErrorCheckOption opts = optss[index];
            opts.SetErrorCheck(ErrorCheckType.NumberStoredAsText, false);
            opts.AddRange(CreateCellArea(&quot;A1&quot;, &quot;D2&quot;));
            opts.AddRange(CreateCellArea(&quot;A3&quot;, &quot;D3&quot;));
            index = optss.Add();
            opts = optss[index];
            opts.SetErrorCheck(ErrorCheckType.TwoDigitTextYear, false);
            opts.SetErrorCheck(ErrorCheckType.NumberStoredAsText, false);
            opts.AddRange(CreateCellArea(&quot;A3&quot;, &quot;D5&quot;));
            workbook.Save(Constants.destPath + &quot;TestErrorCheck.xls&quot;);
            workbook = new Workbook(Constants.destPath + &quot;TestErrorCheck.xls&quot;);
            sheet = workbook.Worksheets[0];
            
            Assert.AreEqual(sheet.ErrorCheckOptions.Count, 2);
            opts = sheet.ErrorCheckOptions[0];
            Assert.AreEqual(opts.GetCountOfRange(), 2);
            Assert.AreEqual(opts.IsErrorCheck(ErrorCheckType.NumberStoredAsText), false);

        }
```

### See Also

* struct [CellArea](../../cellarea/)
* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


