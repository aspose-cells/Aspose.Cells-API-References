---
title: Cells.InsertColumns
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Inserts some columns into the worksheet
type: docs
url: /net/aspose.cells/cells/insertcolumns/
---
## InsertColumns(int, int) {#insertcolumns}

Inserts some columns into the worksheet.

```csharp
public void InsertColumns(int columnIndex, int totalColumns)
```

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | Column index. |
| totalColumns | Int32 | The number of columns. |

### Examples

```csharp
// Called: cells.InsertColumns(16384, 1);
[Test, ExpectedException(typeof(CellsException))]
#endif
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells.InsertColumns(16384, 1);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertColumns(int, int, bool) {#insertcolumns_2}

Inserts some columns into the worksheet.

```csharp
public void InsertColumns(int columnIndex, int totalColumns, bool updateReference)
```

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | Column index. |
| totalColumns | Int32 | The number of columns. |
| updateReference | Boolean | Indicates if references in other worksheets will be updated. |

### Examples

```csharp
// Called: cells.InsertColumns(0, 1, true);
[Test]
        public void Method_Boolean_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "Formula/CellsNet45784.xlsm");
            Cells cells = workbook.Worksheets["Sheet1"].Cells;
            cells.InsertColumns(0, 1, true);
            Assert.AreEqual("{=TABLE(R2,R1)}",cells["O8"].Formula);
	    }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertColumns(int, int, InsertOptions) {#insertcolumns_1}

Inserts some columns into the worksheet.

```csharp
public void InsertColumns(int columnIndex, int totalColumns, InsertOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | Column index. |
| totalColumns | Int32 | The number of columns. |
| options | InsertOptions | The options for inserting operation. |

### See Also

* class [InsertOptions](../../insertoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


