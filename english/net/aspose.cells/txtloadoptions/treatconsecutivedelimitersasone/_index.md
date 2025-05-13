---
title: TxtLoadOptions.TreatConsecutiveDelimitersAsOne
second_title: Aspose.Cells for .NET API Reference
description: TxtLoadOptions property. Whether consecutive delimiters should be treated as one
type: docs
url: /net/aspose.cells/txtloadoptions/treatconsecutivedelimitersasone/
---
## TxtLoadOptions.TreatConsecutiveDelimitersAsOne property

Whether consecutive delimiters should be treated as one.

```csharp
public bool TreatConsecutiveDelimitersAsOne { get; set; }
```

### Examples

```csharp
// Called: tlo.TreatConsecutiveDelimitersAsOne = false;
public void TxtLoadOptions_Property_TreatConsecutiveDelimitersAsOne()
{
    TxtLoadOptions tlo = new TxtLoadOptions(LoadFormat.Csv);
    Workbook wb = LoadAsCsv("1,\"abc\",3,'def'\n\"\"\"g'hi\",,,\n'jkl\"',,,12", tlo);
    Cells cells = wb.Worksheets[0].Cells;
    Assert.AreEqual("abc", cells["B1"].Value, "Default-B1.Value");
    Assert.AreEqual("'def'", cells["D1"].Value, "Default-D1.Value");
    Assert.AreEqual("\"g'hi", cells["A2"].Value, "Default-A2.Value");
    Assert.AreEqual("'jkl\"'", cells["A3"].Value, "Default-D2.Value");
    Assert.AreEqual(CellValueType.IsNull, cells["B3"].Type, "Default-B3.Type");
    Assert.AreEqual(12, cells["D3"].IntValue, "Default-D3.IntValue");

    tlo.TreatConsecutiveDelimitersAsOne = true;
    wb = LoadAsCsv("1,\"abc\",3,'def'\n\"\"\"g'hi\",,,\n'jkl\"',,,12", tlo);
    cells = wb.Worksheets[0].Cells;
    Assert.AreEqual(CellValueType.IsNull, cells["D3"].Type, "ConsecutiveDelimitersAsOne-D3.Type");
    Assert.AreEqual(12, cells["B3"].IntValue, "ConsecutiveDelimitersAsOne-B3.IntValue");

    /*tlo.TreatConsecutiveDelimitersAsOne = true;
    tlo.TextQualifier = '\'';
    ms.Position = 0;
    wb = new Workbook(ms, tlo);
    cells = wb.Worksheets[0].Cells;
    Assert.AreEqual("\"abc\"", cells["B1"].Value, "ConsecutiveDelimitersAsOne&TextQualifier=\"'\"-B1.Value");
    Assert.AreEqual("def", cells["D1"].Value, "ConsecutiveDelimitersAsOne&TextQualifier=\"'\"-D1.Value");
    Assert.AreEqual("\"\"\"g'hi\"", cells["A2"].Value, "ConsecutiveDelimitersAsOne&TextQualifier=\"'\"-A2.Value");
    Assert.AreEqual("jkl\"", cells["A3"].Value, "ConsecutiveDelimitersAsOne&TextQualifier=\"'\"-D2.Value");
    Assert.AreEqual(CellValueType.IsNull, cells["D3"].Type, "ConsecutiveDelimitersAsOne&TextQualifier=\"'\"-D3.Type");
    Assert.AreEqual(12, cells["B3"].IntValue, "ConsecutiveDelimitersAsOne&TextQualifier=\"'\"-B3.IntValue");*/

    tlo = new TxtLoadOptions(LoadFormat.Csv);
    tlo.Encoding = Encoding.Unicode;
    tlo.Separator = ' ';
    wb = LoadAsCsv("1 \"abc\" 3 'def'\n\"\"\"g'hi\"   \n'jkl\"'   12", tlo);
    cells = wb.Worksheets[0].Cells;
    Assert.AreEqual("abc", cells["B1"].Value, "Separator=' '-B1.Value");
    Assert.AreEqual("'def'", cells["D1"].Value, "Separator=' '-D1.Value");
    Assert.AreEqual("\"g'hi", cells["A2"].Value, "Separator=' '-A2.Value");
    Assert.AreEqual("'jkl\"'", cells["A3"].Value, "Separator=' '-D2.Value");
    Assert.AreEqual(CellValueType.IsNull, cells["D3"].Type, "Separator=' '-D3.Type");
    Assert.AreEqual(12, cells["B3"].IntValue, "Separator=' '-B3.IntValue");

    tlo.TreatConsecutiveDelimitersAsOne = false;
    wb = LoadAsCsv("1 \"abc\" 3 'def'\n\"\"\"g'hi\"   \n'jkl\"'   12", tlo);
    cells = wb.Worksheets[0].Cells;
    Assert.AreEqual(CellValueType.IsNull, cells["B3"].Type, "ConsecutiveDelimitersAsOne=false&Separator=' '-B3.Type");
    Assert.AreEqual(12, cells["D3"].IntValue, "ConsecutiveDelimitersAsOne=false&Separator=' '-D3.IntValue");

    tlo = new TxtLoadOptions(LoadFormat.Csv);
    wb = LoadAsCsv("1,\"abc\n 3 'def'\n\"\"ghi", tlo);
    cells = wb.Worksheets[0].Cells;
    Assert.AreEqual("abc\n 3 'def'\n\"ghi", cells["B1"].Value, "Value with multiple lines");
}
```

### See Also

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


