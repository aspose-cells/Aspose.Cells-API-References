---
title: AbstractTextLoadOptions.ConvertDateTimeData
second_title: Aspose.Cells for .NET API Reference
description: AbstractTextLoadOptions property. Gets or sets a value that indicates whether the string in text file is converted to date data
type: docs
url: /net/aspose.cells/abstracttextloadoptions/convertdatetimedata/
---
## AbstractTextLoadOptions.ConvertDateTimeData property

Gets or sets a value that indicates whether the string in text file is converted to date data.

```csharp
public bool ConvertDateTimeData { get; set; }
```

### Examples

```csharp
// Called: tlo.ConvertDateTimeData = false;
public void AbstractTextLoadOptions_Property_ConvertDateTimeData()
{
    TxtLoadOptions tlo = new TxtLoadOptions(LoadFormat.Csv);
    tlo.ConvertNumericData = false;
    tlo.ConvertDateTimeData = false;
    Workbook wb = LoadAsCsv("\"abc\"", tlo);
    Assert.AreEqual("abc", wb.Worksheets[0].Cells[0, 0].Value, "Loaded value");
}
```

### See Also

* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


