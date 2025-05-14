---
title: PivotFieldCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: PivotFieldCollection method. Adds a PivotField Object to the specific type PivotFields
type: docs
url: /net/aspose.cells.pivot/pivotfieldcollection/add/
---
## PivotFieldCollection.Add method

Adds a PivotField Object to the specific type PivotFields.

```csharp
public int Add(PivotField pivotField)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pivotField | PivotField | a PivotField Object. |

### Return Value

the index of the PivotField Object in this PivotFields.

### Examples

```csharp
// Called: pt.ColumnFields.Add(pt.DataField);
public void PivotFieldCollection_Method_Add()
{

    Workbook wb = new Workbook(Constants.openPivottablePath + "test(2).xlsx");
    Worksheet m_currentWorksheet = wb.Worksheets["Data"];

    int startYear = 2009;
    for (int i = 1; i <= 5; i++)
    {
        Cell c = m_currentWorksheet.Cells.Find("LD>>YEAR_" + i, null,null);
        if (c != null)
            c.Value = startYear + (i - 1);
    }

    Random rand = new Random();
    int numRecs = rand.Next(5, 30);
    //int numRecs = 2;
    int templateRow = m_currentWorksheet.Cells.Find("LD>>NAME", null, null).Row;
    for (int j = 0; j < numRecs; j++)
    {
        m_currentWorksheet.Cells.InsertRow(templateRow++);
        m_currentWorksheet.Cells.CopyRow(m_currentWorksheet.Cells, templateRow, templateRow - 1);

        Cell c = m_currentWorksheet.Cells.Find("LD>>NAME", null, null);
        if (c != null)
            c.Value = "Name_" + j;

        for (int k = 1; k <= 5; k++)
        {
            Cell cost = m_currentWorksheet.Cells.Find("LD>>COST_YEAR_" + k, c, null);
            if (cost != null)
                cost.Value = rand.NextDouble() * 10000;
        }
    }

    m_currentWorksheet.Cells.DeleteRow(templateRow);

    m_currentWorksheet = wb.Worksheets["Pivot"];
    PivotTable pt = m_currentWorksheet.PivotTables[0];
    pt.RefreshData();
    //pt.RefreshDataOnOpeningFile = true;
    for (int m = 0; m < 4; m++)
    {
        PivotField field = pt.BaseFields[(startYear + m).ToString()];
        field.SetSubtotals(PivotFieldSubtotalType.Sum, true);
        pt.AddFieldToArea(PivotFieldType.Data, field);
    }
    pt.ColumnFields.Add(pt.DataField);
    pt.CalculateData();
    wb.Save(Constants.savePivottablePath +"example.xlsx");


}
```

### See Also

* class [PivotField](../../pivotfield/)
* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


