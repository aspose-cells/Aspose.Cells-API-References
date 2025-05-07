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
// Called: cells.InsertRange(ca, range.ColumnCount, ShiftType.Right, true);
private static void Method_Boolean_(Aspose.Cells.Range range)
        {
            Cells cells = range.Worksheet.Cells;
            CellArea ca = new CellArea();
            ca.StartRow = range.FirstRow;
            ca.EndRow = cells.MaxRow;
            ca.StartColumn = range.FirstColumn + range.ColumnCount;
            ca.EndColumn = cells.MaxColumn;
            cells.Method_Boolean_(ca, range.ColumnCount, ShiftType.Right, true);
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
// Called: workbook.Worksheets[0].Cells.InsertRange(ca, ShiftType.Down);
[Test]
        public void Method_ShiftType_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet45237.xlsx");
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 2;
            ca.StartColumn = 0;
            ca.EndColumn = 2;

            workbook.Worksheets[0].Cells.InsertRange(ca, ShiftType.Down);
            Assert.AreEqual(3500.0, workbook.Worksheets[0].Cells["B7"].DoubleValue, "B7.Value");
            Assert.AreEqual("{=TABLE(,E2)}", workbook.Worksheets[0].Cells["B8"].Formula, "B8.Formula");
            Assert.AreEqual("{=TABLE(,E2)}", workbook.Worksheets[0].Cells["B9"].Formula, "B9.Formula");
            workbook.Save(Constants.destPath + "CellsNet45237.xlsx");
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
[Test]
        public void Method_ShiftType_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET-43499.xls");
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


