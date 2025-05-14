---
title: PivotTable.ShowInTabularForm
second_title: Aspose.Cells for .NET API Reference
description: PivotTable method. Layouts the PivotTable in tabular form
type: docs
url: /net/aspose.cells.pivot/pivottable/showintabularform/
---
## PivotTable.ShowInTabularForm method

Layouts the PivotTable in tabular form.

```csharp
public void ShowInTabularForm()
```

### Examples

```csharp
// Called: pivotTable.ShowInTabularForm();
private void PivotTable_Method_ShowInTabularForm(Workbook workbook)
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

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


