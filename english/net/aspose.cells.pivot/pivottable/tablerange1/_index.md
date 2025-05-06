---
title: PivotTable.TableRange1
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Returns a CellArea object that represents the range containing the entire PivotTable report but doesnt include page fields. Readonly
type: docs
url: /net/aspose.cells.pivot/pivottable/tablerange1/
---
## PivotTable.TableRange1 property

Returns a CellArea object that represents the range containing the entire PivotTable report, but doesn't include page fields. Read-only.

```csharp
public CellArea TableRange1 { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(39, pt.TableRange1.EndRow);
[Test]
        public void Property_TableRange1()
        {
            Workbook workbook = new Workbook(Constants.PivotTableSourcePath + &quot;CELLSNET-52440.xls&quot;);
            PivotTable pt = workbook.Worksheets[0].PivotTables[0];

            pt.RefreshData();
            pt.CalculateData();
            pt.RefreshDataOnOpeningFile = false;
            workbook.Worksheets[0].Charts[0].RefreshPivotData();
            Assert.AreEqual(39, pt.TableRange1.EndRow);

        }
```

### See Also

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


