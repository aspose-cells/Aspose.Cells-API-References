---
title: PivotTable.DataField
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Gets a PivotField object that represents all the data fields in a PivotTable. Readonly. It would only be created when there are two or more data fields in the Data region. Defaultly it is in row region. You can drag it to the row/column region with PivotTable.AddFieldToArea method 
type: docs
url: /net/aspose.cells.pivot/pivottable/datafield/
---
## PivotTable.DataField property

Gets a [`PivotField`](../../pivotfield/) object that represents all the data fields in a PivotTable. Read-only. It would only be created when there are two or more data fields in the Data region. Defaultly it is in row region. You can drag it to the row/column region with PivotTable.AddFieldToArea() method .

```csharp
public PivotField DataField { get; }
```

### Examples

```csharp
// Called: pt.ColumnFields.Add(pt.DataField);
[Test]
        public void Property_DataField()
        {

            Workbook wb = new Workbook(Constants.openPivottablePath + &quot;test(2).xlsx&quot;);
            Worksheet m_currentWorksheet = wb.Worksheets[&quot;Data&quot;];

            int startYear = 2009;
            for (int i = 1; i &lt;= 5; i++)
            {
                Cell c = m_currentWorksheet.Cells.Find(&quot;LD&gt;&gt;YEAR_&quot; + i, null,null);
                if (c != null)
                    c.Value = startYear + (i - 1);
            }

            Random rand = new Random();
            int numRecs = rand.Next(5, 30);
            //int numRecs = 2;
            int templateRow = m_currentWorksheet.Cells.Find(&quot;LD&gt;&gt;NAME&quot;, null, null).Row;
            for (int j = 0; j &lt; numRecs; j++)
            {
                m_currentWorksheet.Cells.InsertRow(templateRow++);
                m_currentWorksheet.Cells.CopyRow(m_currentWorksheet.Cells, templateRow, templateRow - 1);

                Cell c = m_currentWorksheet.Cells.Find(&quot;LD&gt;&gt;NAME&quot;, null, null);
                if (c != null)
                    c.Value = &quot;Name_&quot; + j;

                for (int k = 1; k &lt;= 5; k++)
                {
                    Cell cost = m_currentWorksheet.Cells.Find(&quot;LD&gt;&gt;COST_YEAR_&quot; + k, c, null);
                    if (cost != null)
                        cost.Value = rand.NextDouble() * 10000;
                }
            }

            m_currentWorksheet.Cells.DeleteRow(templateRow);

            m_currentWorksheet = wb.Worksheets[&quot;Pivot&quot;];
            PivotTable pt = m_currentWorksheet.PivotTables[0];
            pt.RefreshData();
            pt.RefreshDataOnOpeningFile = true;
            for (int m = 0; m &lt; 4; m++)
            {
                PivotField field = pt.BaseFields[(startYear + m).ToString()];
                field.SetSubtotals(PivotFieldSubtotalType.Sum, true);
                pt.AddFieldToArea(PivotFieldType.Data, field);
            }
            pt.ColumnFields.Add(pt.DataField);

            wb.Save(Constants.savePivottablePath + &quot;out.xlsx&quot;);


        }
```

### See Also

* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


