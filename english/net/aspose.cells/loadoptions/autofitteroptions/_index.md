---
title: LoadOptions.AutoFitterOptions
second_title: Aspose.Cells for .NET API Reference
description: LoadOptions property. Gets and sets the auto fitter options
type: docs
url: /net/aspose.cells/loadoptions/autofitteroptions/
---
## LoadOptions.AutoFitterOptions property

Gets and sets the auto fitter options

```csharp
public AutoFitterOptions AutoFitterOptions { get; set; }
```

### Remarks

Only for xlsx ,spreadsheetML file now.

### Examples

```csharp
// Called: loadOptions.AutoFitterOptions.OnlyAuto = true;
[Test]
        public void Property_AutoFitterOptions()
        {
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.AutoFitterOptions = new AutoFitterOptions();
            loadOptions.AutoFitterOptions.OnlyAuto = true;
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsJava41639.xml", loadOptions);
            Assert.AreEqual(workbook.Worksheets[1].Cells.GetColumnWidthPixel(13), 71);
            workbook.Save(Constants.destPath + "CellsJava41638.xlsx");
            workbook = new Workbook(Constants.destPath + "CellsJava41638.xlsx");
            Assert.AreEqual(workbook.Worksheets[0].Cells["I4"].GetStyle().VerticalAlignment, TextAlignmentType.Center);
        }
```

### See Also

* class [AutoFitterOptions](../../autofitteroptions/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


