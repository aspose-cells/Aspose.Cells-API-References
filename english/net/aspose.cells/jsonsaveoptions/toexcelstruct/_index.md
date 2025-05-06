---
title: JsonSaveOptions.ToExcelStruct
second_title: Aspose.Cells for .NET API Reference
description: JsonSaveOptions property. Indicates whether converting to json struct of the Excel file
type: docs
url: /net/aspose.cells/jsonsaveoptions/toexcelstruct/
---
## JsonSaveOptions.ToExcelStruct property

Indicates whether converting to json struct of the Excel file.

```csharp
public bool ToExcelStruct { get; set; }
```

### Remarks

Only for converting range to JSON.

### Examples

```csharp
// Called: saveOptions.ToExcelStruct = true;
[Test]
        public void Property_ToExcelStruct()
        {
            Workbook book = new Workbook(Constants.sourcePath + &quot;CELLSNET55579.xlsx&quot;);
            Aspose.Cells.Range range = book.Worksheets[0].Cells.CreateRange(&quot;A1:B2&quot;);

            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.AlwaysExportAsJsonObject = true;
            saveOptions.ToExcelStruct = true;
            string json = range.ToJson(saveOptions);
            Assert.IsTrue(json.IndexOf(&quot;\&quot;cell\&quot; :&quot;) &gt; 0);
        }
```

### See Also

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


