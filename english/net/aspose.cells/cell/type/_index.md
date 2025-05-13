---
title: Cell.Type
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Represents cell value type
type: docs
url: /net/aspose.cells/cell/type/
---
## Cell.Type property

Represents cell value type.

```csharp
public CellValueType Type { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(CellValueType.IsNumeric, cells[0, 0].Type, "A1");
public void Cell_Property_Type()
{
    Workbook wb = new Workbook();
    wb.Settings.Region = CountryCode.USA;
    Cells cells = wb.Worksheets[0].Cells;
    cells[0, 0].PutValue("1.2345");
    cells[0, 1].PutValue("1,2345");
    cells = wb.Worksheets.Add("Sheet2").Cells;
    TxtLoadOptions tlo = new TxtLoadOptions(LoadFormat.Csv);
    tlo.Region = CountryCode.USA;
    tlo.Encoding = Encoding.Unicode;
    MemoryStream ms = new MemoryStream(Encoding.Unicode.GetBytes("\"1.2345\",\"1,2345\",\"1.2.3456\",\"True\",\"False\""), false);
    cells.ImportCSV(ms, tlo, 0, 0);
    tlo.Region = CountryCode.Germany;
    ms.Seek(0, SeekOrigin.Begin);
    cells.ImportCSV(ms, tlo, 1, 0);
    Assert.AreEqual(CellValueType.IsNumeric, cells[0, 0].Type, "A1");
    Assert.AreEqual(CellValueType.IsNumeric, cells[0, 1].Type, "B1"); //before 24.2 it is string
    Assert.AreEqual(CellValueType.IsString, cells[0, 2].Type, "C1");
    Assert.IsTrue(cells[0, 3].BoolValue, "D1");
    Assert.IsFalse(cells[0, 4].BoolValue, "E1");
    Assert.AreEqual(CellValueType.IsNumeric, cells[1, 0].Type, "A2"); //before 24.2 it is datetime
    Assert.AreEqual(CellValueType.IsNumeric, cells[1, 1].Type, "B1");
    Assert.AreEqual(CellValueType.IsDateTime, cells[1, 2].Type, "C2");
    Assert.IsTrue(cells[1, 3].BoolValue, "D2");
    Assert.IsFalse(cells[1, 4].BoolValue, "E2");
}
```

### See Also

* enum [CellValueType](../../cellvaluetype/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


