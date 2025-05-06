---
title: PivotField.DisplayName
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Represents the PivotField display name
type: docs
url: /net/aspose.cells.pivot/pivotfield/displayname/
---
## PivotField.DisplayName property

Represents the PivotField display name.

```csharp
public string DisplayName { get; set; }
```

### Examples

```csharp
// Called: pivotDataFields[&amp;quot;ChangeInExp&amp;quot;].DisplayName = &amp;quot;Change In Exp&amp;quot;;
[Test]
        public void Property_DisplayName()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET45313_&quot;;

                  

            string mFullFilePath = filePath + &quot;Sample without Pivots.xlsx&quot;;
            string outFilePath = CreateFolder(filePath) + &quot;out.xlsx&quot;;


            //Open workbook
            Aspose.Cells.Workbook workbook = new Aspose.Cells.Workbook();
            Aspose.Cells.Worksheet worksheet;
            Aspose.Cells.WorksheetCollection worksheets;
            //Aspose.Cells.Range range;
            //Aspose.Cells.Cells cells;
            char[] splitchar = { &apos;:&apos; };


            //Open workbook
            workbook = new Aspose.Cells.Workbook(mFullFilePath);

            //Calculate any formulas in the workbook
            workbook.CalculateFormula();

            worksheets = workbook.Worksheets;

            foreach (Aspose.Cells.Worksheet ws in workbook.Worksheets)
            {
                //Freeze top row
                ws.FreezePanes(1, 0, 1, 0);

                //Autofit all columns and rows
                ws.AutoFitColumns();
                ws.AutoFitRows();
            }

            Aspose.Cells.Worksheet detailWorksheet;
            Aspose.Cells.Pivot.PivotTableCollection pivotTables;
            Aspose.Cells.Pivot.PivotTable pivotTable;
            Aspose.Cells.Pivot.PivotField pivotField;
            Aspose.Cells.Pivot.PivotItemCollection pivotItems;
            Aspose.Cells.Pivot.PivotItem pivotItem;
            //Aspose.Cells.Pivot.PivotFieldCollection pivotColumnFields;
            Aspose.Cells.Pivot.PivotFieldCollection pivotDataFields;
            //Aspose.Cells.Pivot.PivotFieldCollection pivotPageFields;

            int pivotTableIndex;

            //Pivot Table font style
            Aspose.Cells.Style style = workbook.CreateStyle();
            style.Font.Size = 9;
            style.Font.Name = &quot;Calibri&quot;;



            // Begin GL Audit Summary Pivot Table

            Console.WriteLine(&quot;{0} Begin GL Audit Summary pivot&quot;, DateTime.Now.ToString());

            detailWorksheet = workbook.Worksheets[&quot;GL Audit Detail&quot;];

            worksheet = workbook.Worksheets.Add(&quot;GL Audit Summary&quot;);
            worksheet.MoveTo(0);

            pivotTables = worksheet.PivotTables;

            pivotTableIndex = pivotTables.Add(string.Format(&quot;&apos;GL Audit Detail&apos;!A1:{0}&quot;, CellsHelper.CellIndexToName(detailWorksheet.Cells.MaxDataRow, 30)), &quot;A1&quot;, &quot;PivotTable1&quot;);

            pivotTable = pivotTables[pivotTableIndex];

            pivotTable.PivotTableStyleType = Aspose.Cells.Pivot.PivotTableStyleType.PivotTableStyleLight16;

            pivotTable.ShowValuesRow = false;

            //Remove Grand Total
            pivotTable.ShowRowGrandTotals = false;


            //RowFields
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, &quot;ProgramName&quot;);

            //Uncheck &quot;(blank)&quot; item
            pivotField = pivotTable.RowFields[&quot;ProgramName&quot;];
            pivotField.IsAutoSort = true;
            pivotField.IsAscendSort = true;
            pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

            pivotItems = pivotField.PivotItems;

            if (pivotItems.Count &gt; 1)
            {

                for (int i = 0; i &lt; pivotItems.Count; i++)
                {
                    pivotItem = pivotItems[i];
                    if (pivotItem.Name != null)
                    {
                        if (pivotItem.Name.Equals(&quot;(blank)&quot;))
                        {
                            pivotItem.IsHidden = true;
                        }
                    }
                }
            }

            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, &quot;PolicyNumber&quot;);

            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, &quot;InsuredName&quot;);
            //Hide Subtotal
            pivotField = pivotTable.RowFields[&quot;InsuredName&quot;];
            pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, &quot;EffDate&quot;);
            //Hide Subtotal
            pivotField = pivotTable.RowFields[&quot;EffDate&quot;];
            pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, &quot;ExpDate&quot;);
            //Hide Subtotal
            pivotField = pivotTable.RowFields[&quot;ExpDate&quot;];
            pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, &quot;RiskState&quot;);
            //Hide Subtotal
            pivotField = pivotTable.RowFields[&quot;RiskState&quot;];
            pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, &quot;ExpBasis&quot;);
            //Hide Subtotal
            pivotField = pivotTable.RowFields[&quot;ExpBasis&quot;];
            pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, &quot;FirstAuditRevNumber&quot;);
            //Hide Subtotal
            pivotField = pivotTable.RowFields[&quot;FirstAuditRevNumber&quot;];
            pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, &quot;FirstAuditAgingDays&quot;);
            //Hide Subtotal
            pivotField = pivotTable.RowFields[&quot;FirstAuditAgingDays&quot;];
            pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, &quot;SecondAuditRevNumber&quot;);
            //Hide Subtotal
            pivotField = pivotTable.RowFields[&quot;SecondAuditRevNumber&quot;];
            pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, &quot;SecondAuditAgingDays&quot;);
            //Hide Subtotal
            pivotField = pivotTable.RowFields[&quot;SecondAuditAgingDays&quot;];
            pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, &quot;ThirdAuditRevNumber&quot;);
            //Hide Subtotal
            pivotField = pivotTable.RowFields[&quot;ThirdAuditRevNumber&quot;];
            pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, &quot;ThirdAuditAgingDays&quot;);
            //Hide Subtotal
            pivotField = pivotTable.RowFields[&quot;ThirdAuditAgingDays&quot;];
            pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, &quot;Class&quot;);
            //Hide Subtotal
            pivotField = pivotTable.RowFields[&quot;Class&quot;];
            pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, &quot;ClassDescription&quot;);
            //Hide Subtotal
            pivotField = pivotTable.RowFields[&quot;ClassDescription&quot;];
            pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

            //DataFields
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, &quot;ExposureAtInception&quot;);
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, &quot;ExposureAtAudit&quot;);

            pivotTable.AddCalculatedField(&quot;ChangeInExp&quot;, &quot;=IF(ExposureAtAudit=0,IF(ExposureAtInception=0,0,-1),IF(ExposureAtInception=0,1,(ExposureAtAudit-ExposureAtInception)/ExposureAtInception))&quot;);

            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, &quot;WrittenPremiumAtInception&quot;);
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, &quot;WrittenPremiumAllEndorsements&quot;);
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, &quot;PremiumAtAudit&quot;);

            pivotTable.AddCalculatedField(&quot;ChangeInPrem&quot;, &quot;=IF(PremiumAtAudit=0,IF(WrittenPremiumAtInception=0,0,-1),IF(WrittenPremiumAtInception=0,IF(PremiumAtAudit&lt;0,(PremiumAtAudit/PremiumAtAudit)*-1,(PremiumAtAudit/PremiumAtAudit)),(PremiumAtAudit-WrittenPremiumAtInception)/WrittenPremiumAtInception))&quot;);

            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Column, pivotTable.DataField);

            //Update Captions and NumberFormats
            pivotDataFields = pivotTable.DataFields;

            pivotDataFields[&quot;ExposureAtInception&quot;].DisplayName = &quot;Exposure At Inception&quot;;
            pivotDataFields[&quot;ExposureAtInception&quot;].NumberFormat = &quot;$#,##0.00_);[Red]($#,##0.00)&quot;;

            pivotDataFields[&quot;ExposureAtAudit&quot;].DisplayName = &quot;Exposure At Audit&quot;;
            pivotDataFields[&quot;ExposureAtAudit&quot;].NumberFormat = &quot;$#,##0.00_);[Red]($#,##0.00)&quot;;

            pivotDataFields[&quot;ChangeInExp&quot;].DisplayName = &quot;Change In Exp&quot;;
            pivotDataFields[&quot;ChangeInExp&quot;].NumberFormat = &quot;0.0%;[Red](0.0%)&quot;;

            pivotDataFields[&quot;WrittenPremiumAtInception&quot;].DisplayName = &quot;Premium At Inception&quot;;
            pivotDataFields[&quot;WrittenPremiumAtInception&quot;].NumberFormat = &quot;$#,##0.00_);[Red]($#,##0.00)&quot;;

            pivotDataFields[&quot;WrittenPremiumAllEndorsements&quot;].DisplayName = &quot;Premium All Endorsements&quot;;
            pivotDataFields[&quot;WrittenPremiumAllEndorsements&quot;].NumberFormat = &quot;$#,##0.00_);[Red]($#,##0.00)&quot;;

            pivotDataFields[&quot;PremiumAtAudit&quot;].DisplayName = &quot;Premium At Audit&quot;;
            pivotDataFields[&quot;PremiumAtAudit&quot;].NumberFormat = &quot;$#,##0.00_);[Red]($#,##0.00)&quot;;

            pivotDataFields[&quot;ChangeInPrem&quot;].DisplayName = &quot;Change In Prem&quot;;
            pivotDataFields[&quot;ChangeInPrem&quot;].NumberFormat = &quot;0.0%;[Red](0.0%)&quot;;


            pivotTable.FormatAll(style);

            //pivotTable.IsGridDropZones = true;
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            pivotTable.RefreshDataOnOpeningFile = true;

            //Autofit all columns and rows
            worksheet.AutoFitColumns();
            worksheet.AutoFitRows();

            Console.WriteLine(&quot;{0} End GL Audit Summary pivot&quot;, DateTime.Now.ToString());

            // End GL Audit Summary Pivot Table


            // Begin GL Audit Totals Pivot Table

            Console.WriteLine(&quot;{0} Begin GL Audit Totals pivot&quot;, DateTime.Now.ToString());

            worksheet = workbook.Worksheets.Add(&quot;GL Audit Totals&quot;);
            worksheet.MoveTo(workbook.Worksheets[&quot;GL Audit Summary&quot;].Index + 1);

            detailWorksheet = workbook.Worksheets[&quot;GL Audit Detail&quot;];

            pivotTables = worksheet.PivotTables;

            pivotTableIndex = pivotTables.Add(string.Format(&quot;&apos;GL Audit Detail&apos;!A1:{0}&quot;, CellsHelper.CellIndexToName(detailWorksheet.Cells.MaxDataRow, 30)), &quot;A1&quot;, &quot;PivotTable2&quot;);

            pivotTable = pivotTables[pivotTableIndex];


            //RowFields
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, &quot;ProgramName&quot;);

            //Uncheck &quot;(blank)&quot; item
            pivotField = pivotTable.RowFields[&quot;ProgramName&quot;];
            pivotField.IsAutoSort = true;
            pivotField.IsAscendSort = true;

            pivotItems = pivotField.PivotItems;

            if (pivotItems.Count &gt; 1)
            {

                for (int i = 0; i &lt; pivotItems.Count; i++)
                {
                    pivotItem = pivotItems[i];
                    if (pivotItem.Name != null)
                    {
                        if (pivotItem.Name.Equals(&quot;(blank)&quot;))
                        {
                            pivotItem.IsHidden = true;
                        }
                    }
                }
            }


            //DataFields
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, &quot;ExposureAtInception&quot;);
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, &quot;ExposureAtAudit&quot;);

            /*
                THE CODE IS FAILING ON THE FOLLOWING LINE

                From what I can tell, it is due to me re-using the exact same cell range from the previous pivot table

                pivotTableIndex = pivotTables.Add(string.Format(&quot;&apos;GL Audit Detail&apos;!A1:{0}&quot;, CellsHelper.CellIndexToName(detailWorksheet.Cells.MaxDataRow, 30)), &quot;A1&quot;, &quot;PivotTable2&quot;);

                If I change the column 30 to something else, like 31, the following line of code does not generate the error
            */
            pivotTable.AddCalculatedField(&quot;ChangeInExp&quot;, &quot;=IF(ExposureAtAudit=0,IF(ExposureAtInception=0,0,-1),IF(ExposureAtInception=0,1,(ExposureAtAudit-ExposureAtInception)/ExposureAtInception))&quot;);

            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, &quot;WrittenPremiumAtInception&quot;);
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, &quot;WrittenPremiumAllEndorsements&quot;);
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, &quot;PremiumAtAudit&quot;);

            pivotTable.AddCalculatedField(&quot;ChangeInPrem&quot;, &quot;=IF(PremiumAtAudit=0,IF(WrittenPremiumAtInception=0,0,-1),IF(WrittenPremiumAtInception=0,IF(PremiumAtAudit&lt;0,(PremiumAtAudit/PremiumAtAudit)*-1,(PremiumAtAudit/PremiumAtAudit)),(PremiumAtAudit-WrittenPremiumAtInception)/WrittenPremiumAtInception))&quot;);


            //Update Captions and NumberFormats
            pivotDataFields = pivotTable.DataFields;

            pivotDataFields[&quot;ExposureAtInception&quot;].DisplayName = &quot;Exposure At Inception&quot;;
            pivotDataFields[&quot;ExposureAtInception&quot;].NumberFormat = &quot;$#,##0.00_);[Red]($#,##0.00)&quot;;

            pivotDataFields[&quot;ExposureAtAudit&quot;].DisplayName = &quot;Exposure At Audit&quot;;
            pivotDataFields[&quot;ExposureAtAudit&quot;].NumberFormat = &quot;$#,##0.00_);[Red]($#,##0.00)&quot;;

            pivotDataFields[&quot;ChangeInExp&quot;].DisplayName = &quot;Change In Exp&quot;;
            pivotDataFields[&quot;ChangeInExp&quot;].NumberFormat = &quot;0.0%;[Red](0.0%)&quot;;

            pivotDataFields[&quot;WrittenPremiumAtInception&quot;].DisplayName = &quot;Premium At Inception&quot;;
            pivotDataFields[&quot;WrittenPremiumAtInception&quot;].NumberFormat = &quot;$#,##0.00_);[Red]($#,##0.00)&quot;;

            pivotDataFields[&quot;WrittenPremiumAllEndorsements&quot;].DisplayName = &quot;Premium All Endorsements&quot;;
            pivotDataFields[&quot;WrittenPremiumAllEndorsements&quot;].NumberFormat = &quot;$#,##0.00_);[Red]($#,##0.00)&quot;;

            pivotDataFields[&quot;PremiumAtAudit&quot;].DisplayName = &quot;Premium At Audit&quot;;
            pivotDataFields[&quot;PremiumAtAudit&quot;].NumberFormat = &quot;$#,##0.00_);[Red]($#,##0.00)&quot;;

            pivotDataFields[&quot;ChangeInPrem&quot;].DisplayName = &quot;Change In Prem&quot;;
            pivotDataFields[&quot;ChangeInPrem&quot;].NumberFormat = &quot;0.0%;[Red](0.0%)&quot;;


            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Column, pivotTable.DataField);

            pivotTable.PivotTableStyleType = Aspose.Cells.Pivot.PivotTableStyleType.PivotTableStyleLight16;

            pivotTable.ShowValuesRow = false;

            //Remove Grand Total
            pivotTable.ShowRowGrandTotals = false;


            pivotTable.FormatAll(style);

            //pivotTable.IsGridDropZones = true;

       
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            pivotTable.RefreshDataOnOpeningFile = true;

            //Autofit all columns and rows
            worksheet.AutoFitColumns();
            worksheet.AutoFitRows();

            Console.WriteLine(&quot;{0} End GL Audit Totals pivot&quot;, DateTime.Now.ToString());

            // End GL Audit Totals Pivot Table


            // Begin GL Audit History Summary Pivot Table

            Console.WriteLine(&quot;{0} Begin GL Audit History Summary pivot&quot;, DateTime.Now.ToString());

            detailWorksheet = workbook.Worksheets[&quot;GL Audit History Detail&quot;];

            worksheet = workbook.Worksheets.Add(&quot;GL Audit History Summary&quot;);
            worksheet.MoveTo(workbook.Worksheets[&quot;GL Audit Totals&quot;].Index + 1);

            pivotTables = worksheet.PivotTables;

            pivotTableIndex = pivotTables.Add(string.Format(&quot;&apos;GL Audit History Detail&apos;!A1:{0}&quot;, CellsHelper.CellIndexToName(detailWorksheet.Cells.MaxDataRow, 30)), &quot;A1&quot;, &quot;PivotTable3&quot;);

            pivotTable = pivotTables[pivotTableIndex];

            pivotTable.PivotTableStyleType = Aspose.Cells.Pivot.PivotTableStyleType.PivotTableStyleLight16;

            pivotTable.ShowValuesRow = false;

            //Remove Grand Total
            pivotTable.ShowRowGrandTotals = false;


            //RowFields
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, &quot;ProgramName&quot;);

            //Uncheck &quot;(blank)&quot; item
            pivotField = pivotTable.RowFields[&quot;ProgramName&quot;];
            pivotField.IsAutoSort = true;
            pivotField.IsAscendSort = true;
            pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

            pivotItems = pivotField.PivotItems;

            if (pivotItems.Count &gt; 1)
            {

                for (int i = 0; i &lt; pivotItems.Count; i++)
                {
                    pivotItem = pivotItems[i];
                    if (pivotItem.Name != null)
                    {
                        if (pivotItem.Name.Equals(&quot;(blank)&quot;))
                        {
                            pivotItem.IsHidden = true;
                        }
                    }
                }
            }

            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, &quot;PolicyNumber&quot;);
            //Hide Subtotal
            pivotField = pivotTable.RowFields[&quot;PolicyNumber&quot;];
            pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, &quot;InsuredName&quot;);
            //Hide Subtotal
            pivotField = pivotTable.RowFields[&quot;InsuredName&quot;];
            pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, &quot;EffDate&quot;);
            //Hide Subtotal
            pivotField = pivotTable.RowFields[&quot;EffDate&quot;];
            pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, &quot;ExpDate&quot;);
            //Hide Subtotal
            pivotField = pivotTable.RowFields[&quot;ExpDate&quot;];
            pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, &quot;RiskState&quot;);
            //Hide Subtotal
            pivotField = pivotTable.RowFields[&quot;RiskState&quot;];
            pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, &quot;ExpBasis&quot;);
            //Hide Subtotal
            pivotField = pivotTable.RowFields[&quot;ExpBasis&quot;];
            pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, &quot;FirstAuditRevNumber&quot;);
            //Hide Subtotal
            pivotField = pivotTable.RowFields[&quot;FirstAuditRevNumber&quot;];
            pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, &quot;FirstAuditAgingDays&quot;);
            //Hide Subtotal
            pivotField = pivotTable.RowFields[&quot;FirstAuditAgingDays&quot;];
            pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, &quot;SecondAuditRevNumber&quot;);
            //Hide Subtotal
            pivotField = pivotTable.RowFields[&quot;SecondAuditRevNumber&quot;];
            pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, &quot;SecondAuditAgingDays&quot;);
            //Hide Subtotal
            pivotField = pivotTable.RowFields[&quot;SecondAuditAgingDays&quot;];
            pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, &quot;ThirdAuditRevNumber&quot;);
            //Hide Subtotal
            pivotField = pivotTable.RowFields[&quot;ThirdAuditRevNumber&quot;];
            pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, &quot;ThirdAuditAgingDays&quot;);
            //Hide Subtotal
            pivotField = pivotTable.RowFields[&quot;ThirdAuditAgingDays&quot;];
            pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);


            //DataFields
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, &quot;ExposureAtInception&quot;);
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, &quot;ExposureAtAudit&quot;);

            pivotTable.AddCalculatedField(&quot;ChangeInExp&quot;, &quot;=IF(ExposureAtAudit=0,IF(ExposureAtInception=0,0,-1),IF(ExposureAtInception=0,1,(ExposureAtAudit-ExposureAtInception)/ExposureAtInception))&quot;);

            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, &quot;WrittenPremiumAtInception&quot;);
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, &quot;WrittenPremiumAllEndorsements&quot;);
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, &quot;PremiumAtAudit&quot;);

            pivotTable.AddCalculatedField(&quot;ChangeInPrem&quot;, &quot;=IF(PremiumAtAudit=0,IF(WrittenPremiumAtInception=0,0,-1),IF(WrittenPremiumAtInception=0,IF(PremiumAtAudit&lt;0,(PremiumAtAudit/PremiumAtAudit)*-1,(PremiumAtAudit/PremiumAtAudit)),(PremiumAtAudit-WrittenPremiumAtInception)/WrittenPremiumAtInception))&quot;);

            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Column, pivotTable.DataField);

            //Update Captions and NumberFormats
            pivotDataFields = pivotTable.DataFields;

            pivotDataFields[&quot;ExposureAtInception&quot;].DisplayName = &quot;Exposure At Inception&quot;;
            pivotDataFields[&quot;ExposureAtInception&quot;].NumberFormat = &quot;$#,##0.00_);[Red]($#,##0.00)&quot;;

            pivotDataFields[&quot;ExposureAtAudit&quot;].DisplayName = &quot;Exposure At Audit&quot;;
            pivotDataFields[&quot;ExposureAtAudit&quot;].NumberFormat = &quot;$#,##0.00_);[Red]($#,##0.00)&quot;;

            pivotDataFields[&quot;ChangeInExp&quot;].DisplayName = &quot;Change In Exp&quot;;
            pivotDataFields[&quot;ChangeInExp&quot;].NumberFormat = &quot;0.0%;[Red](0.0%)&quot;;

            pivotDataFields[&quot;WrittenPremiumAtInception&quot;].DisplayName = &quot;Premium At Inception&quot;;
            pivotDataFields[&quot;WrittenPremiumAtInception&quot;].NumberFormat = &quot;$#,##0.00_);[Red]($#,##0.00)&quot;;

            pivotDataFields[&quot;WrittenPremiumAllEndorsements&quot;].DisplayName = &quot;Premium All Endorsements&quot;;
            pivotDataFields[&quot;WrittenPremiumAllEndorsements&quot;].NumberFormat = &quot;$#,##0.00_);[Red]($#,##0.00)&quot;;

            pivotDataFields[&quot;PremiumAtAudit&quot;].DisplayName = &quot;Premium At Audit&quot;;
            pivotDataFields[&quot;PremiumAtAudit&quot;].NumberFormat = &quot;$#,##0.00_);[Red]($#,##0.00)&quot;;

            pivotDataFields[&quot;ChangeInPrem&quot;].DisplayName = &quot;Change In Prem&quot;;
            pivotDataFields[&quot;ChangeInPrem&quot;].NumberFormat = &quot;0.0%;[Red](0.0%)&quot;;


            pivotTable.FormatAll(style);

            //pivotTable.IsGridDropZones = true;

            pivotTable.RefreshData();
            pivotTable.CalculateData();
            pivotTable.RefreshDataOnOpeningFile = true;

            //Autofit all columns and rows
            worksheet.AutoFitColumns();
            worksheet.AutoFitRows();

            Console.WriteLine(&quot;{0} End GL Audit History Summary pivot&quot;, DateTime.Now.ToString());

            // End GL Audit History Summary Pivot Table


            // Begin GL Audit History Totals Pivot Table

            Console.WriteLine(&quot;{0} Begin GL Audit History Totals pivot&quot;, DateTime.Now.ToString());

            detailWorksheet = workbook.Worksheets[&quot;GL Audit History Detail&quot;];

            worksheet = workbook.Worksheets.Add(&quot;GL Audit History Totals&quot;);
            worksheet.MoveTo(workbook.Worksheets[&quot;GL Audit History Summary&quot;].Index + 1);

            pivotTables = worksheet.PivotTables;

            pivotTableIndex = pivotTables.Add(string.Format(&quot;&apos;GL Audit History Detail&apos;!A1:{0}&quot;, CellsHelper.CellIndexToName(detailWorksheet.Cells.MaxDataRow, 30)), &quot;A1&quot;, &quot;PivotTable4&quot;);

            pivotTable = pivotTables[pivotTableIndex];

            pivotTable.PivotTableStyleType = Aspose.Cells.Pivot.PivotTableStyleType.PivotTableStyleLight16;

            pivotTable.ShowValuesRow = false;

            //Remove Grand Total
            pivotTable.ShowRowGrandTotals = false;

            //RowFields
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, &quot;ProgramName&quot;);

            //Uncheck &quot;(blank)&quot; item
            pivotField = pivotTable.RowFields[&quot;ProgramName&quot;];
            pivotField.IsAutoSort = true;
            pivotField.IsAscendSort = true;
            pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

            pivotItems = pivotField.PivotItems;

            if (pivotItems.Count &gt; 1)
            {

                for (int i = 0; i &lt; pivotItems.Count; i++)
                {
                    pivotItem = pivotItems[i];
                    if (pivotItem.Name != null)
                    {
                        if (pivotItem.Name.Equals(&quot;(blank)&quot;))
                        {
                            pivotItem.IsHidden = true;
                        }
                    }
                }
            }


            //DataFields
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, &quot;ExposureAtInception&quot;);
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, &quot;ExposureAtAudit&quot;);

            pivotTable.AddCalculatedField(&quot;ChangeInExp&quot;, &quot;=IF(ExposureAtAudit=0,IF(ExposureAtInception=0,0,-1),IF(ExposureAtInception=0,1,(ExposureAtAudit-ExposureAtInception)/ExposureAtInception))&quot;);

            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, &quot;WrittenPremiumAtInception&quot;);
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, &quot;WrittenPremiumAllEndorsements&quot;);
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, &quot;PremiumAtAudit&quot;);

            pivotTable.AddCalculatedField(&quot;ChangeInPrem&quot;, &quot;=IF(PremiumAtAudit=0,IF(WrittenPremiumAtInception=0,0,-1),IF(WrittenPremiumAtInception=0,IF(PremiumAtAudit&lt;0,(PremiumAtAudit/PremiumAtAudit)*-1,(PremiumAtAudit/PremiumAtAudit)),(PremiumAtAudit-WrittenPremiumAtInception)/WrittenPremiumAtInception))&quot;);

            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Column, pivotTable.DataField);

            //Update Captions and NumberFormats
            pivotDataFields = pivotTable.DataFields;

            pivotDataFields[&quot;ExposureAtInception&quot;].DisplayName = &quot;Exposure At Inception&quot;;
            pivotDataFields[&quot;ExposureAtInception&quot;].NumberFormat = &quot;$#,##0.00_);[Red]($#,##0.00)&quot;;

            pivotDataFields[&quot;ExposureAtAudit&quot;].DisplayName = &quot;Exposure At Audit&quot;;
            pivotDataFields[&quot;ExposureAtAudit&quot;].NumberFormat = &quot;$#,##0.00_);[Red]($#,##0.00)&quot;;

            pivotDataFields[&quot;ChangeInExp&quot;].DisplayName = &quot;Change In Exp&quot;;
            pivotDataFields[&quot;ChangeInExp&quot;].NumberFormat = &quot;0.0%;[Red](0.0%)&quot;;

            pivotDataFields[&quot;WrittenPremiumAtInception&quot;].DisplayName = &quot;Premium At Inception&quot;;
            pivotDataFields[&quot;WrittenPremiumAtInception&quot;].NumberFormat = &quot;$#,##0.00_);[Red]($#,##0.00)&quot;;

            pivotDataFields[&quot;WrittenPremiumAllEndorsements&quot;].DisplayName = &quot;Premium All Endorsements&quot;;
            pivotDataFields[&quot;WrittenPremiumAllEndorsements&quot;].NumberFormat = &quot;$#,##0.00_);[Red]($#,##0.00)&quot;;

            pivotDataFields[&quot;PremiumAtAudit&quot;].DisplayName = &quot;Premium At Audit&quot;;
            pivotDataFields[&quot;PremiumAtAudit&quot;].NumberFormat = &quot;$#,##0.00_);[Red]($#,##0.00)&quot;;

            pivotDataFields[&quot;ChangeInPrem&quot;].DisplayName = &quot;Change In Prem&quot;;
            pivotDataFields[&quot;ChangeInPrem&quot;].NumberFormat = &quot;0.0%;[Red](0.0%)&quot;;


            pivotTable.FormatAll(style);

            //pivotTable.IsGridDropZones = true;

           
            pivotTable.RefreshData();
            pivotTable.CalculateData();
          
            pivotTable.RefreshDataOnOpeningFile = true;

            //Autofit all columns and rows
            worksheet.AutoFitColumns();
            worksheet.AutoFitRows();

            Console.WriteLine(&quot;{0} End GL Audit History Totals pivot&quot;, DateTime.Now.ToString());

            workbook.Save(outFilePath);
        }
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


