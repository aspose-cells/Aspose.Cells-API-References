---
title: Style.Custom
second_title: Aspose.Cells for .NET API Reference
description: Style property. Represents the custom number format string of this style object. If the custom number format is not setFor example the number format is builtin  will be returned
type: docs
url: /net/aspose.cells/style/custom/
---
## Style.Custom property

Represents the custom number format string of this style object. If the custom number format is not set(For example, the number format is builtin), "" will be returned.

```csharp
public string Custom { get; set; }
```

### Remarks

The returned custom string is culture-independent.

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Worksheets[0].Cells[0, 0].GetStyle().Custom, "M/D/YYYY".ToLower());
[Test, Category("Bug")]
        public void Property_Custom()
        {
            Workbook workbook = new Workbook();
            TxtLoadOptions loadOptions = new TxtLoadOptions();
            loadOptions.Separator = ',';
            //workbook.Open(Constants.sourcePath + "CsvInput.csv",',');
            workbook = new Workbook(Constants.sourcePath + "CsvInput.csv", loadOptions);
            Assert.AreEqual(workbook.Worksheets[0].Cells[0, 0].GetStyle().Custom, "M/D/YYYY".ToLower());
            Assert.AreEqual(workbook.Worksheets[0].Cells[0, 2].GetStyle().Custom, "YYYY-M-D".ToLower());
        }
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


