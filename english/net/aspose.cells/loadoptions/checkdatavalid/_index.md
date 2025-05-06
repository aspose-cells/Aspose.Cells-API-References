---
title: LoadOptions.CheckDataValid
second_title: Aspose.Cells for .NET API Reference
description: LoadOptions property. Check whether data is valid in the template file
type: docs
url: /net/aspose.cells/loadoptions/checkdatavalid/
---
## LoadOptions.CheckDataValid property

Check whether data is valid in the template file.

```csharp
public bool CheckDataValid { get; set; }
```

### Examples

```csharp
// Called: options.CheckDataValid = true;
[Test]
        public void Property_CheckDataValid()
        {
            LoadOptions options = new LoadOptions();
            options.CheckDataValid = true;
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSJAVA-43118.xls&quot;, options);
            workbook.Save(Constants.destPath + &quot;CELLSJAVA-43118.pdf&quot;);
        }
```

### See Also

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


