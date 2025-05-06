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
// Called: sourceCells.InsertRange(ca, 1, ShiftType.Down, true);
public static void Method_Boolean_()
        {
            WorkbookDesigner designer = new WorkbookDesigner();
            Workbook workbook = new Workbook(USBankConstants.sourcePath + &quot;InsertInRangeAndIndex.xlsx&quot;);
            designer.Workbook = workbook;

            Cells sourceCells = workbook.Worksheets[0].Cells;
            Aspose.Cells.Range sourceRange = sourceCells.CreateRange(0, 0, 1, 1);

            CellArea ca = new CellArea();
            ca.StartRow = 1;
            ca.EndRow = ca.StartRow;
            ca.StartColumn = 0;
            ca.EndColumn = 0;
            sourceCells.InsertRange(ca, 1, ShiftType.Down, true);

            string output = USBankConstants.resultPath + &quot;InsertInRangeAndIndex_result.xlsx&quot;;
            workbook.Save(output);
           
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
[Test]
        public void Method_ShiftType_()
        {
            caseName = &quot;testInsertRangeFormual_054&quot;;
            Workbook workbook = new Workbook();
            workbook = new Workbook(Constants.sourcePath + &quot;insertDelete\\testformual3.xls&quot;);
            Cells cells = workbook.Worksheets[0].Cells;
            CellArea cellarea = common.setCellArea(4, 6, 5, 7);
            cells.InsertRange(cellarea, ShiftType.Down);

            checkInsertRangeFormual(workbook);
            workbook.Save(Constants.destPath + &quot;testInsertRangeFormual.xls&quot;);
            workbook = new Workbook(Constants.destPath + &quot;testInsertRangeFormual.xls&quot;);
            checkInsertRangeFormual(workbook);
            workbook.Save(Constants.destPath + &quot;testInsertRangeFormual.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;testInsertRangeFormual.xlsx&quot;);
            checkInsertRangeFormual(workbook);
            workbook.Save(Constants.destPath + &quot;testInsertRangeFormual.xml&quot;, SaveFormat.SpreadsheetML);
            workbook = new Workbook(Constants.destPath + &quot;testInsertRangeFormual.xml&quot;);
            checkInsertRangeFormual(workbook);
            workbook.Save(Constants.destPath + &quot;testInsertRangeFormual.xls&quot;);
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
// Called: xlWorkSheet.Cells.InsertRange(xlMonthCArea, 3, ShiftType.Right);
[Test]
        public void Method_ShiftType_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;Test_162926.xls&quot;);
            Worksheet xlWorkSheet = workbook.Worksheets[0];
            CellArea xlMonthCArea = new CellArea();
            xlMonthCArea.StartRow = 9;
            xlMonthCArea.EndRow = 127;
            xlMonthCArea.StartColumn = 10;
            xlMonthCArea.EndColumn = 10;

            xlWorkSheet.Cells.InsertRange(xlMonthCArea, 3, ShiftType.Right);

            workbook.Save(Constants.destPath + &quot;Test_162926.xls&quot;);
        }
```

### See Also

* struct [CellArea](../../cellarea/)
* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


