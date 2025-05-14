---
title: AbstractTextLoadOptions.ConvertNumericData
second_title: Aspose.Cells for .NET API Reference
description: AbstractTextLoadOptions property. Gets or sets a value that indicates whether the string in text file is converted to numeric data
type: docs
url: /net/aspose.cells/abstracttextloadoptions/convertnumericdata/
---
## AbstractTextLoadOptions.ConvertNumericData property

Gets or sets a value that indicates whether the string in text file is converted to numeric data.

```csharp
public bool ConvertNumericData { get; set; }
```

### Examples

```csharp
// Called: tlo.ConvertNumericData = true;
public void AbstractTextLoadOptions_Property_ConvertNumericData()
{
    TxtLoadOptions tlo = new TxtLoadOptions(LoadFormat.Csv);
    tlo.ConvertNumericData = true;
    tlo.ConvertDateTimeData = true;
    tlo.HasFormula = true;
    StringBuilder sb = new StringBuilder(300);
    sb.Append("=\"abcde");
    for (int i = 0; i < 25; i++)
    {
        sb.Append("0123456789");
    }
    sb.Append('"');
    string fml = sb.ToString();
    Workbook wb = LoadAsCsv(fml, tlo);
    Assert.AreEqual(fml, wb.Worksheets[0].Cells[0, 0].Formula, "Loaded formula for valid formula string");
    sb.Insert(sb.Length - 1, "f");
    fml = sb.ToString();
    wb = LoadAsCsv(fml, tlo);
    Assert.IsFalse(wb.Worksheets[0].Cells[0, 0].IsFormula, "Loaded cell for invalid formula string should not be formula");
    Assert.AreEqual(fml, wb.Worksheets[0].Cells[0, 0].Value, "Loaded value for invalid formula string");
}
```

### See Also

* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


