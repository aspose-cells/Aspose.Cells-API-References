---
title: Cell.GetCharacters
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Returns all Characters objects that represents a range of characters within the cell text
type: docs
url: /net/aspose.cells/cell/getcharacters/
---
## GetCharacters() {#getcharacters}

Returns all Characters objects that represents a range of characters within the cell text.

```csharp
public FontSetting[] GetCharacters()
```

### Return Value

All Characters objects

### Examples

```csharp
// Called: FontSetting[] fs = cell.GetCharacters();
[Test]
        public void Method_GetCharacters()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSJAVA45154.xls");
            Cell cell = workbook.Worksheets[2].Cells["D1"];
            FontSetting[] fs = cell.GetCharacters();
            Assert.AreEqual(FontUnderlineType.Single, fs[0].Font.Underline);
            Assert.AreEqual(FontUnderlineType.None, fs[1].Font.Underline);
        }
```

### See Also

* class [FontSetting](../../fontsetting/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetCharacters(bool) {#getcharacters_1}

Returns all Characters objects that represents a range of characters within the cell text.

```csharp
public FontSetting[] GetCharacters(bool flag)
```

| Parameter | Type | Description |
| --- | --- | --- |
| flag | Boolean | Indicates whether applying table style to the cell if the cell is in the table. |

### Return Value

All Characters objects

### Examples

```csharp
// Called: FontSetting[] fs = cell.GetCharacters(true);
[Test]
        public void Method_Boolean_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet44480.xlsx");
            Cell cell = workbook.Worksheets[0].Cells["C8"];
            FontSetting[] fs = cell.GetCharacters(true);
            for (int i = 0; i < fs.Length; i++)
            {
               AssertHelper.AreEqual(Color.White, fs[i].Font.Color);
            }
        }
```

### See Also

* class [FontSetting](../../fontsetting/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


