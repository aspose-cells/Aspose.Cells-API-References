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
// Called: Assert.AreEqual(pivotTable.TableRange1.EndRow, 3);
private void PivotTable_Property_TableRange1(Workbook workbook)
        {
            var pivotSheet = workbook.Worksheets.Add("Pivot");
            var pivotTableIndex = pivotSheet.PivotTables.Add("=Data!A1:B3", "A1", "PivotTable1");
            var pivotTable = pivotSheet.PivotTables[pivotTableIndex];
            var labelFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Label");
            var labelField = pivotTable.RowFields[labelFieldIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            pivotTable.ShowInTabularForm();
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            Assert.AreEqual(pivotTable.TableRange1.StartRow, 0);
            Assert.AreEqual(pivotTable.TableRange1.EndRow, 3);
            Assert.AreEqual(pivotTable.TableRange1.StartColumn, 0);
            Assert.AreEqual(pivotTable.TableRange1.EndColumn, 1);
            Assert.AreEqual(pivotSheet.Cells["A1"].StringValue, "Label");
            Assert.AreEqual(pivotSheet.Cells["B1"].StringValue, "Count of Value");

            // These should cause us to use the "tabular" form but we'll still get the "Row Labels" behavior.
            labelField.ShowCompact = false;
            labelField.ShowInOutlineForm = false;
            // pivotTable.ShowInTabularForm();
            pivotTable.RefreshDataOnOpeningFile = false;
        }
```

### See Also

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


