---
title: LoadOptions.KeepUnparsedData
second_title: Aspose.Cells for .NET API Reference
description: LoadOptions property. Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. Default is true
type: docs
url: /net/aspose.cells/loadoptions/keepunparseddata/
---
## LoadOptions.KeepUnparsedData property

Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. Default is true.

```csharp
public bool KeepUnparsedData { get; set; }
```

### Remarks

For scenarios that user only needs to read some contents from template file and does not need to save the workbook back, set this property as false may improve performance, especially when using it together with some kind of LoadFilter,

### Examples

```csharp
// Called: options.KeepUnparsedData = false;
[Test]
        public void Property_KeepUnparsedData()
        {
            LoadOptions options = new LoadOptions();
            options.ParsingFormulaOnOpen = false;
            options.KeepUnparsedData = false;
            options.CheckDataValid = false;
            options.CheckExcelRestriction = false;

            String[] files = {&quot;JAVA45489-1.xlsx&quot;, &quot;JAVA45489-1.xlsx&quot;, &quot;JAVA45489-1.xlsx&quot;};

            foreach (String fileName in files)
            {
                Workbook wb = new Workbook(Constants.sourcePath + fileName, options);
                wb.Save(Constants.destPath + fileName.Substring(0, fileName.IndexOf(&quot;.&quot;)) + &quot;_JAVA45489.xls&quot;);
            }
        }
```

### See Also

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


