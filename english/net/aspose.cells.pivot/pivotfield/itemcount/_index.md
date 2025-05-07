---
title: PivotField.ItemCount
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Gets the count of the base items in this pivot field
type: docs
url: /net/aspose.cells.pivot/pivotfield/itemcount/
---
## PivotField.ItemCount property

Gets the count of the base items in this pivot field.

```csharp
public int ItemCount { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(6,pt.BaseFields["Seneste aktivitetsdato"].ItemCount);
[Test]
        public void Property_ItemCount()
        {
            string filePath = Constants.PivotTableSourcePath + "NET50329_";
            string savePath = CreateFolder(filePath);
            Workbook wb = new Workbook(filePath + "S.xls");
            PivotTable pt = wb.Worksheets["SidsteKontakt"].PivotTables[0];
            Assert.AreEqual(6,pt.BaseFields["Seneste aktivitetsdato"].ItemCount);
            wb.Save(savePath + "S_out.xlsx");
            wb.Save(savePath + "S_out.xlsb");

            wb = new Workbook(savePath + "S_out.xlsb");
            Assert.AreEqual(wb.Worksheets[1].PivotTables[0].DataSource[0], "Tabel__01intranote_IntraNoteITP_CRM_ActivityLogAll[#Alt]");
        }
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


