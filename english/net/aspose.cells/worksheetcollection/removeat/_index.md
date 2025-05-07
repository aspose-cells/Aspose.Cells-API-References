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
// Called: wb.Worksheets.RemoveAt(sourceWorksheet.Name);
[Test]
        public void Method_String_()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "CellsNet45261.xlsx");
            var sourceWorksheet = wb.Worksheets[0];
            Worksheet newWorksheet = wb.Worksheets.Add("NewCopySheet");
            newWorksheet.MoveTo(sourceWorksheet.Index + 1);
            newWorksheet.Copy(sourceWorksheet);
            wb.Worksheets.RemoveAt(sourceWorksheet.Name);
            // wb.Worksheets.RemoveAt(sourceWorksheet.Name);
            Assert.AreEqual(newWorksheet.Cells["D2"].Formula, "=IF(IF(ISBLANK([@[Current Projected End Date]]),0,DAYS([@[Current Projected End Date]],[@[Original Projected End Date]]))<0,0,IF(ISBLANK([@[Current Projected End Date]]),0,DAYS([@[Current Projected End Date]],[@[Original Projected End Date]])))");
            wb.Save(Constants.destPath + "CellsNet45261.xlsx");
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
// Called: workbook.Worksheets.RemoveAt(0);
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET49523.xlsx");
            workbook.Worksheets.RemoveAt(0);
            workbook.Worksheets.Clear();
            workbook.Worksheets.Add();
            workbook.Worksheets[0].Name = "test";
            Assert.AreEqual(0, workbook.Worksheets.Names.Count);
            workbook.Save(Constants.destPath + "CELLSNET49523.xlsx");
        }
```

### See Also

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


