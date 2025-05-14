---
title: Cells.InsertRange
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Inserts a range of cells and shift cells according to the shift option
type: docs
url: /net/aspose.cells/cells/insertrange/
---
## InsertRange(CellArea, int, ShiftType, bool) {#insertrange_2}

Inserts a range of cells and shift cells according to the shift option.

```csharp
public void InsertRange(CellArea area, int shiftNumber, ShiftType shiftType, bool updateReference)
```

| Parameter | Type | Description |
| --- | --- | --- |
| area | CellArea | Shift area. |
| shiftNumber | Int32 | Number of rows or columns to be inserted. |
| shiftType | ShiftType | Shift cells option. |
| updateReference | Boolean | Indicates whether update references in other worksheets. |

### Examples

```csharp
// Called: cells.InsertRange(area, 1, ShiftType.Right, true);
private static void Cells_Method_InsertRange(Cells cells, int row)
        {

            CellArea area = CellArea.CreateCellArea(row, 1, row + 1, 1);
            cells.InsertRange(area, 1, ShiftType.Right, true);
            Aspose.Cells.Range sourceRange = cells.CreateRange(row, 0, 2, 1);
            Aspose.Cells.Range targetRange = cells.CreateRange(row, 1, 2, 1);
            targetRange.Copy(sourceRange);
        }
```

### See Also

* struct [CellArea](../../cellarea/)
* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertRange(CellArea, ShiftType) {#insertrange}

Inserts a range of cells and shift cells according to the shift option.

```csharp
public void InsertRange(CellArea area, ShiftType shiftType)
```

| Parameter | Type | Description |
| --- | --- | --- |
| area | CellArea | Shift area. |
| shiftType | ShiftType | Shift cells option. |

### Examples

```csharp
// Called: cells.InsertRange(cellarea, ShiftType.Down);
public void Cells_Method_InsertRange()
{
    caseName = "testInsertRangeStyle_036";
    Workbook workbook = new Workbook(Constants.sourcePath + "insertDelete\\testStyle.xls");
    Cells cells = workbook.Worksheets[0].Cells;
    CellArea cellarea = common.setCellArea(1, 5, 2, 5);
    cells.InsertRange(cellarea, ShiftType.Down);

    checkInsertRangeStyle_036(workbook);
    workbook.Save(Constants.destPath + "testInsertRangeStyle.xls");
    workbook = new Workbook(Constants.destPath + "testInsertRangeStyle.xls");
    checkInsertRangeStyle_036(workbook);
    workbook.Save(Constants.destPath + "testInsertRangeStyle.xlsx");
    workbook = new Workbook(Constants.destPath + "testInsertRangeStyle.xlsx");
    checkInsertRangeStyle_036(workbook);
    workbook.Save(Constants.destPath + "testInsertRangeStyle.xml", SaveFormat.SpreadsheetML);
    workbook = new Workbook(Constants.destPath + "testInsertRangeStyle.xml", new LoadOptions(LoadFormat.SpreadsheetML));
    checkInsertRangeStyle_036(workbook);
    workbook.Save(Constants.destPath + "testInsertRangeStyle.xls");
}
```

### See Also

* struct [CellArea](../../cellarea/)
* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertRange(CellArea, int, ShiftType) {#insertrange_1}

Inserts a range of cells and shift cells according to the shift option.

```csharp
public void InsertRange(CellArea area, int shiftNumber, ShiftType shiftType)
```

| Parameter | Type | Description |
| --- | --- | --- |
| area | CellArea | Shift area. |
| shiftNumber | Int32 | Number of rows or columns to be inserted. |
| shiftType | ShiftType | Shift cells option. |

### Examples

```csharp
// Called: workbook.Worksheets["Tables"].Cells.InsertRange(objCellArea, 1, ShiftType.Right);
public void Cells_Method_InsertRange()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    CellArea objCellArea = new CellArea();

    objCellArea.StartColumn = 1;

    objCellArea.StartRow = 0;

    objCellArea.EndColumn = 1;

    objCellArea.EndRow = 0;


    workbook.Worksheets["Tables"].Cells.InsertRange(objCellArea, 1, ShiftType.Right);


    workbook.Worksheets["Tables"].AutoFitRow(0);
}
```

### See Also

* struct [CellArea](../../cellarea/)
* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


