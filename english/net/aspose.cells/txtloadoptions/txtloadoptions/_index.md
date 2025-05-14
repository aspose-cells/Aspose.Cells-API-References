---
title: TxtLoadOptions.TxtLoadOptions
second_title: Aspose.Cells for .NET API Reference
description: TxtLoadOptions constructor. Creates the options for loading text file
type: docs
url: /net/aspose.cells/txtloadoptions/txtloadoptions/
---
## TxtLoadOptions() {#constructor}

Creates the options for loading text file.

```csharp
public TxtLoadOptions()
```

### Remarks

The default load file type is CSV .

### Examples

```csharp
// Called: TxtLoadOptions loadOptions = new TxtLoadOptions();
[Test, Category("Bug")]
        public void TxtLoadOptions_Constructor()
        {
            Workbook workbook = new Workbook();
            //workbook.Open(Constants.sourcePath + "example.csv", ',');           
            TxtLoadOptions loadOptions = new TxtLoadOptions();
            loadOptions.Separator = ',';
            workbook = new Workbook(Constants.sourcePath + "example.csv", loadOptions);
            Assert.IsTrue(workbook.Worksheets[0].Cells["A5"].GetStyle().IsDateTime);
            // Assert.AreEqual(workbook.Worksheets[0].Cells[0, 2].GetStyle().Custom, "YYYY-M-D".ToLower());
        }
```

### See Also

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## TxtLoadOptions(LoadFormat) {#constructor_1}

Creates the options for loading text file.

```csharp
public TxtLoadOptions(LoadFormat loadFormat)
```

| Parameter | Type | Description |
| --- | --- | --- |
| loadFormat | LoadFormat | The loading format |

### See Also

* enum [LoadFormat](../../loadformat/)
* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


