---
title: WorksheetCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection property. Gets the Worksheet element at the specified index
type: docs
url: /net/aspose.cells/worksheetcollection/item/
---
## WorksheetCollection indexer (1 of 2)

Gets the [`Worksheet`](../../worksheet/) element at the specified index.

```csharp
public Worksheet this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |

### Return Value

The element at the specified index.

### Examples

```csharp
// Called: Worksheet sheet = workbook.Worksheets[0];
[Test]
       public void Property_Int32_()
       {
           Workbook workbook = new Workbook(FileFormatType.Xlsx);
           Worksheet sheet = workbook.Worksheets[0];
           sheet.Validations.Add(CellArea.CreateCellArea("A1","A1"));
           sheet.Validations[0].Type = ValidationType.List;
           sheet.Validations[0].Formula1 = "=B1:B2";
           sheet.Cells["B1"].PutValue("A");
           sheet.Cells["B2"].PutValue("B");
           object t = sheet.Validations[0].Value1;
           Assert.AreEqual("A", ((object[])t)[0].ToString());
       }
```

### See Also

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## WorksheetCollection indexer (2 of 2)

Gets the [`Worksheet`](../../worksheet/) element with the specified name.

```csharp
public Worksheet this[string sheetName] { get; }
```

| Parameter | Description |
| --- | --- |
| sheetName | Worksheet name |

### Return Value

The element with the specified name.

### Examples

```csharp
// Called: Worksheet sheet = workbook.Worksheets["sheetDest"];
private void Property_String_(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets["sheetDest"];
            testAreEqual(0, sheet.Comments.Count, caseName);
        }
```

### See Also

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


