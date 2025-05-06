---
title: WorksheetCollection.AddCopy
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection method. Adds a worksheet to the collection and copies data from an existed worksheet
type: docs
url: /net/aspose.cells/worksheetcollection/addcopy/
---
## AddCopy(string) {#addcopy_1}

Adds a worksheet to the collection and copies data from an existed worksheet.

```csharp
public int AddCopy(string sheetName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sheetName | String | Name of source worksheet. |

### Return Value

[`Worksheet`](../../worksheet/) object index.

### Exceptions

| exception | condition |
| --- | --- |
| [CellsException](../../cellsexception/) | Specifies an invalid worksheet name. |

### Examples

```csharp
// Called: workbook.Worksheets.AddCopy(worksheet.Name);
[Test]
        public void Method_String_()
        {
            var workbook = new Workbook();
            var worksheet = workbook.Worksheets[0];
            var list = worksheet.ListObjects[worksheet.ListObjects.Add(0, 0, 4, 4, false)];
            worksheet.Slicers.Add(list, list.ListColumns[0], 8, 8);
            workbook.Worksheets.AddCopy(worksheet.Name);
            Assert.AreEqual(&quot;Column1 1&quot;, workbook.Worksheets[1].Shapes[0].Name);
            Assert.AreEqual(&quot;Column1 1&quot;, workbook.Worksheets[1].Slicers[0].Name);
            workbook.Save(Constants.destPath + &quot;CELLSNET56102.xlsx&quot;);
        }
```

### See Also

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddCopy(int) {#addcopy}

Adds a worksheet to the collection and copies data from an existed worksheet.

```csharp
public int AddCopy(int sheetIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sheetIndex | Int32 | Index of source worksheet. |

### Return Value

[`Worksheet`](../../worksheet/) object index.

### Examples

```csharp
// Called: int index = wb.Worksheets.AddCopy(0);
[Test]
        public void Method_Int32_()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;Net49739.xlsx&quot;);
            int index = wb.Worksheets.AddCopy(0);
            Assert.AreEqual(1, wb.Worksheets[index].ConditionalFormattings.Count);

            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Copy(wb.Worksheets[0]);
            Assert.AreEqual(0, workbook.Worksheets[0].ConditionalFormattings.Count);
        }
```

### See Also

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddCopy(Worksheet[], string[]) {#addcopy_2}

Copy a group of worksheets.

```csharp
public void AddCopy(Worksheet[] source, string[] destSheetNames)
```

| Parameter | Type | Description |
| --- | --- | --- |
| source | Worksheet[] | The source worksheets. |
| destSheetNames | String[] | The names of the copied sheets. |

### See Also

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


