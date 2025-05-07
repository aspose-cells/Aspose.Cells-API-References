---
title: NameCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: NameCollection property. Gets the Name element at the specified index
type: docs
url: /net/aspose.cells/namecollection/item/
---
## NameCollection indexer (1 of 2)

Gets the [`Name`](../../name/) element at the specified index.

```csharp
public Name this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |

### Return Value

The element at the specified index.

### Examples

```csharp
// Called: Assert.AreEqual("='”'!$A$1:$C$6", workbook.Worksheets.Names[1].RefersTo);
[Test]
        public void Property_Int32_()
        {
            //='"'!$A$1:$C$7
            Workbook workbook = new Workbook(Constants.sourcePath + "Formula/CELLSNET44884.xlsx");
            Assert.AreEqual("='\"'!$A$1:$C$7", workbook.Worksheets.Names[0].RefersTo);
            Assert.AreEqual("='”'!$A$1:$C$6", workbook.Worksheets.Names[1].RefersTo);
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
        }
```

### See Also

* class [Name](../../name/)
* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## NameCollection indexer (2 of 2)

Gets the [`Name`](../../name/) element with the specified name.

```csharp
public Name this[string text] { get; }
```

| Parameter | Description |
| --- | --- |
| text | Name text. |

### Return Value

The element with the specified name.

### Examples

```csharp
// Called: workbook.Worksheets.Names[myKey].Text = "I99_999_9999_103";
[Test]
        public void Property_String_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet44240.xls");
            Worksheet aSheet = workbook.Worksheets[0];

            string myKey = aSheet.Name + "!I02_ARSET_52050_103";
            string myNewKey = aSheet.Name + "!I99_999_9999_103";

            workbook.Worksheets.Names[myKey].Text = "I99_999_9999_103";

            //Now I should have in my namecollection the new name but if I try to find new name it is null 
            Name nome2 = workbook.Worksheets.Names[myNewKey];
            Assert.IsTrue(nome2 != null);
            Name nome3 = workbook.Worksheets.Names[myKey];
            Assert.IsTrue(nome3 == null);//
        }
```

### See Also

* class [Name](../../name/)
* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


