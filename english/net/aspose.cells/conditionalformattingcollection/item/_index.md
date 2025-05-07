---
title: ConditionalFormattingCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: ConditionalFormattingCollection property. Gets the FormatConditions element at the specified index
type: docs
url: /net/aspose.cells/conditionalformattingcollection/item/
---
## ConditionalFormattingCollection indexer

Gets the FormatConditions element at the specified index.

```csharp
public FormatConditionCollection this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |

### Examples

```csharp
// Called: FormatConditionCollection fcc = cfc[cfc.Add()];
[Test]
        public void Property_Int32_()
        {
            Workbook wb = new Workbook();
            ConditionalFormattingCollection cfc = wb.Worksheets[0].ConditionalFormattings;
            FormatConditionCollection fcc = cfc[cfc.Add()];
            FormatCondition fc = fcc[fcc.AddCondition(FormatConditionType.NotContainsBlanks)];
            fc.Style.Font.Size = 26;
            fcc.AddArea(CellArea.CreateCellArea(0, 5, 0, 6));
            fcc.AddArea(CellArea.CreateCellArea(3, 0, 4, 0));
            Cell cell = wb.Worksheets[0].Cells[0, 5];
            cell.PutValue(1);
            Assert.AreEqual(26, cell.GetDisplayStyle().Font.Size, "F1.DisplayStyle before saving");
            MemoryStream ms = new MemoryStream(16384);
            wb.Save(ms, SaveFormat.Xlsx);
            ms.Position = 0;
            ManualFileUtil.ManualCheckStringInZip(ms, "xl/worksheets/sheet1.xml",
                new string[] { "LEN(TRIM(A1))&gt;0" }, true);
            ms.Position = 0;
            wb = new Workbook(ms);
            Assert.AreEqual(26, wb.Worksheets[0].Cells[0, 5].GetDisplayStyle().Font.Size,
                "F1.DisplayStyle after re-saving");
        }
```

### See Also

* class [FormatConditionCollection](../../formatconditioncollection/)
* class [ConditionalFormattingCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


