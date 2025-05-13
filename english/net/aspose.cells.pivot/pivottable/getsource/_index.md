---
title: PivotTable.GetSource
second_title: Aspose.Cells for .NET API Reference
description: PivotTable method. Get pivottables source data
type: docs
url: /net/aspose.cells.pivot/pivottable/getsource/
---
## GetSource() {#getsource}

Get pivottable's source data.

```csharp
public string[] GetSource()
```

### Examples

```csharp
// Called: Assert.AreEqual("MyRange", workbook.Worksheets["Sheet1"].PivotTables["PivotTable1"].GetSource()[0]);
public void PivotTable_Method_GetSource()
{
    Workbook workbook = new Workbook(Constants.PivotTableSourcePath + "example.xlsx");
    workbook.Worksheets["Sheet1"].PivotTables["PivotTable1"].ChangeDataSource(new[] { "MyRange" });
    Assert.AreEqual("MyRange", workbook.Worksheets["Sheet1"].PivotTables["PivotTable1"].GetSource()[0]);
    workbook.Save(Constants.PivotTableDestPath + "example.xlsx");
    workbook = new Workbook(Constants.PivotTableDestPath + "example.xlsx");
    Assert.AreEqual("MyRange", workbook.Worksheets["Sheet1"].PivotTables["PivotTable1"].GetSource()[0]);
}
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GetSource(bool) {#getsource_1}

Get pivottable's source data.

```csharp
public string[] GetSource(bool isOriginal)
```

| Parameter | Type | Description |
| --- | --- | --- |
| isOriginal | Boolean | Indicates whether to return original or display data source |

### Examples

```csharp
// Called: string org = pt.GetSource(true)[0];
public void PivotTable_Method_GetSource()
{
    Workbook workbook = new Workbook(Constants.PivotTableSourcePath + "example.xlsx");
    PivotTable pt = workbook.Worksheets[0].PivotTables[0];
    string org = pt.GetSource(true)[0];
    Assert.IsTrue(org.StartsWith(@"'\sites\"));
    string source = pt.GetSource(false)[0];
    Assert.IsTrue(source.StartsWith(@"'https:"));
    workbook.Save(Constants.PivotTableDestPath + "example.xlsx");
}
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


