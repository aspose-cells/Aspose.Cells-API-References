---
title: WorkbookSettings.WarningCallback
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Gets or sets warning callback
type: docs
url: /net/aspose.cells/workbooksettings/warningcallback/
---
## WorkbookSettings.WarningCallback property

Gets or sets warning callback.

```csharp
public IWarningCallback WarningCallback { get; set; }
```

### Examples

```csharp
// Called: wb.Settings.WarningCallback = new CustomWarningCallback(wb);
[Test]
        public void Property_WarningCallback()
        {
            var wb = new Workbook(Constants.sourcePath + &quot;Cells47415.xlsx&quot;);
            wb.Settings.WarningCallback = new CustomWarningCallback(wb);
            var headerSourceWs = wb.Worksheets[&quot;_sheetname_&quot;];
            var dataSourceWs = wb.Worksheets[&quot;firstsheet&quot;];
            //2. copy and rename to create &quot;secondsheet&quot;
            var outputWs = wb.Worksheets[wb.Worksheets.AddCopy(dataSourceWs.Index)];
            outputWs.Name = &quot;secondsheet&quot;;
            //3. copy the first row from _sheetname_ to secondsheet
            outputWs.Cells.CopyRows(headerSourceWs.Cells, 0, 0, 1);
            ////4. recalculate and save out
            //wb.CalculateFormula(new CalculationOptions { IgnoreError = true, Recursive = true });
            //outputWs.Cells[&quot;G1&quot;].Calculate(new CalculationOptions { Recursive = true, IgnoreError = true });
            ////Output 1 - does not recalculate
            //wb.Save(dir + &quot;dest.pdf&quot;);
            Assert.AreEqual(&quot;=named.range_1&quot;, outputWs.Cells[&quot;G1&quot;].Formula);
            Util.ReSave(wb, SaveFormat.Xlsx);
            //wb.Save(Constants.destPath + &quot;Cells47415.xlsx&quot;);
        }
```

### See Also

* interface [IWarningCallback](../../iwarningcallback/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


