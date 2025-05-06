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
private void Method_ShowInTabularForm(Workbook workbook)
        {
            var pivotSheet = workbook.Worksheets.Add(&quot;Pivot&quot;);
            var pivotTableIndex = pivotSheet.PivotTables.Add(&quot;=Data!A1:B3&quot;, &quot;A1&quot;, &quot;PivotTable1&quot;);
            var pivotTable = pivotSheet.PivotTables[pivotTableIndex];
            var labelFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, &quot;Label&quot;);
            var labelField = pivotTable.RowFields[labelFieldIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Data, &quot;Value&quot;);
            pivotTable.ShowInTabularForm();
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            Assert.AreEqual(pivotTable.TableRange1.StartRow, 0);
            Assert.AreEqual(pivotTable.TableRange1.EndRow, 3);
            Assert.AreEqual(pivotTable.TableRange1.StartColumn, 0);
            Assert.AreEqual(pivotTable.TableRange1.EndColumn, 1);
            Assert.AreEqual(pivotSheet.Cells[&quot;A1&quot;].StringValue, &quot;Label&quot;);
            Assert.AreEqual(pivotSheet.Cells[&quot;B1&quot;].StringValue, &quot;Count of Value&quot;);

            // These should cause us to use the &quot;tabular&quot; form but we&apos;ll still get the &quot;Row Labels&quot; behavior.
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


