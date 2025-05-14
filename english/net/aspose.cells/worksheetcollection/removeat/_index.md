---
title: WorksheetCollection.RemoveAt
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection method. Removes the element at a specified name
type: docs
url: /net/aspose.cells/worksheetcollection/removeat/
---
## RemoveAt(string) {#removeat_2}

Removes the element at a specified name.

```csharp
public void RemoveAt(string name)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the element to remove. |

### Examples

```csharp
// Called: wb.Worksheets.RemoveAt("Sheet3");
public void WorksheetCollection_Method_RemoveAt()
{
    Workbook wb = new Workbook();
    wb.Worksheets.Add("Sheet2");
    wb.Worksheets.Add("Sheet3");
    wb.Worksheets.Names[wb.Worksheets.Names.Add("testname")].RefersTo = "=[Book1.xlsx]Sheet1!$A1";
    wb.Worksheets.Names[wb.Worksheets.Names.Add("Sheet2!testname")].RefersTo = "=[Book1.xlsx]Sheet2!$A2";
    wb.Worksheets[1].Cells[0, 0].SetSharedFormula("=testname", 10, 1);
    wb.Worksheets[2].Cells[0, 0].SetSharedFormula("=testname", 10, 1);
    wb.Worksheets.Add();
    wb.Worksheets.ExternalLinks.Clear();
    wb.Worksheets.RemoveAt("Sheet1");
    wb.Worksheets.RemoveAt("Sheet2");
    wb.Worksheets.RemoveAt("Sheet3");
    wb.Save(new MemoryStream(), SaveFormat.Xlsx);
}
```

### See Also

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RemoveAt(int) {#removeat}

Removes the element at a specified index.

```csharp
public void RemoveAt(int index)
```

| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The index value of the element to remove. |

### Examples

```csharp
// Called: wb.Worksheets.RemoveAt(ws.Index);
public void WorksheetCollection_Method_RemoveAt()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsm");
    Worksheet ws = wb.Worksheets["Second"];
    wb.Worksheets.RemoveAt(ws.Index);
    Assert.AreEqual(wb.VbaProject.Modules.Count , 3);
    wb.Save(Constants.destPath + "example.xlsm");
}
```

### See Also

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


