---
title: PivotTable.AddCalculatedField
second_title: Aspose.Cells for .NET API Reference
description: PivotTable method. Adds a calculated field to pivot field
type: docs
url: /net/aspose.cells.pivot/pivottable/addcalculatedfield/
---
## AddCalculatedField(string, string, bool) {#addcalculatedfield_1}

Adds a calculated field to pivot field.

```csharp
public void AddCalculatedField(string name, string formula, bool dragToDataArea)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the calculated field |
| formula | String | The formula of the calculated field. |
| dragToDataArea | Boolean | True,drag this field to data area immediately |

### Examples

```csharp
// Called: pt.AddCalculatedField("testcalfld", "=Sales*2", true);
public void PivotTable_Method_AddCalculatedField()
{
    string filePath = Constants.PivotTableSourcePath + @"NET50981_";

    Workbook wb = new Workbook(filePath + "calField.xlsx");
    Worksheet sheet = wb.Worksheets[0];
    PivotTableCollection pivotTables = sheet.PivotTables;
    PivotTable pt = pivotTables[0];
    pt.AddCalculatedField("testcalfld", "=Sales*2", true);

}
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## AddCalculatedField(string, string) {#addcalculatedfield}

Adds a calculated field to pivot field and drag it to data area.

```csharp
public void AddCalculatedField(string name, string formula)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the calculated field |
| formula | String | The formula of the calculated field. |

### Examples

```csharp
// Called: pivotTable.AddCalculatedField("ChangeInPrem", "=IF(PremiumAtAudit=0,IF(WrittenPremiumAtInception=0,0,-1),IF(WrittenPremiumAtInception=0,IF(PremiumAtAudit<0,(PremiumAtAudit/PremiumAtAudit)*-1,(PremiumAtAudit/PremiumAtAudit)),(PremiumAtAudit-WrittenPremiumAtInception)/WrittenPremiumAtInception))");
public void PivotTable_Method_AddCalculatedField()
{
    string filePath = Constants.PivotTableSourcePath + @"NET45313_";

                  

    string mFullFilePath = filePath + "Sample without Pivots.xlsx";
    string outFilePath = CreateFolder(filePath) + "out.xlsx";


    //Open workbook
    Aspose.Cells.Workbook workbook = new Aspose.Cells.Workbook();
    Aspose.Cells.Worksheet worksheet;
    Aspose.Cells.WorksheetCollection worksheets;
    //Aspose.Cells.Range range;
    //Aspose.Cells.Cells cells;
    char[] splitchar = { ':' };


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
    style.Font.Name = "Calibri";



    // Begin GL Audit Summary Pivot Table

    Console.WriteLine("{0} Begin GL Audit Summary pivot", DateTime.Now.ToString());

    detailWorksheet = workbook.Worksheets["GL Audit Detail"];

    worksheet = workbook.Worksheets.Add("GL Audit Summary");
    worksheet.MoveTo(0);

    pivotTables = worksheet.PivotTables;

    pivotTableIndex = pivotTables.Add(string.Format("'GL Audit Detail'!A1:{0}", CellsHelper.CellIndexToName(detailWorksheet.Cells.MaxDataRow, 30)), "A1", "PivotTable1");

    pivotTable = pivotTables[pivotTableIndex];

    pivotTable.PivotTableStyleType = Aspose.Cells.Pivot.PivotTableStyleType.PivotTableStyleLight16;

    pivotTable.ShowValuesRow = false;

    //Remove Grand Total
    pivotTable.ShowRowGrandTotals = false;


    //RowFields
    pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, "ProgramName");

    //Uncheck "(blank)" item
    pivotField = pivotTable.RowFields["ProgramName"];
    pivotField.IsAutoSort = true;
    pivotField.IsAscendSort = true;
    pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

    pivotItems = pivotField.PivotItems;

    if (pivotItems.Count > 1)
    {

        for (int i = 0; i < pivotItems.Count; i++)
        {
            pivotItem = pivotItems[i];
            if (pivotItem.Name != null)
            {
                if (pivotItem.Name.Equals("(blank)"))
                {
                    pivotItem.IsHidden = true;
                }
            }
        }
    }

    pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, "PolicyNumber");

    pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, "InsuredName");
    //Hide Subtotal
    pivotField = pivotTable.RowFields["InsuredName"];
    pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

    pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, "EffDate");
    //Hide Subtotal
    pivotField = pivotTable.RowFields["EffDate"];
    pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

    pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, "ExpDate");
    //Hide Subtotal
    pivotField = pivotTable.RowFields["ExpDate"];
    pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

    pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, "RiskState");
    //Hide Subtotal
    pivotField = pivotTable.RowFields["RiskState"];
    pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

    pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, "ExpBasis");
    //Hide Subtotal
    pivotField = pivotTable.RowFields["ExpBasis"];
    pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

    pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, "FirstAuditRevNumber");
    //Hide Subtotal
    pivotField = pivotTable.RowFields["FirstAuditRevNumber"];
    pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

    pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, "FirstAuditAgingDays");
    //Hide Subtotal
    pivotField = pivotTable.RowFields["FirstAuditAgingDays"];
    pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

    pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, "SecondAuditRevNumber");
    //Hide Subtotal
    pivotField = pivotTable.RowFields["SecondAuditRevNumber"];
    pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

    pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, "SecondAuditAgingDays");
    //Hide Subtotal
    pivotField = pivotTable.RowFields["SecondAuditAgingDays"];
    pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

    pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, "ThirdAuditRevNumber");
    //Hide Subtotal
    pivotField = pivotTable.RowFields["ThirdAuditRevNumber"];
    pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

    pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, "ThirdAuditAgingDays");
    //Hide Subtotal
    pivotField = pivotTable.RowFields["ThirdAuditAgingDays"];
    pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

    pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, "Class");
    //Hide Subtotal
    pivotField = pivotTable.RowFields["Class"];
    pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

    pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, "ClassDescription");
    //Hide Subtotal
    pivotField = pivotTable.RowFields["ClassDescription"];
    pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

    //DataFields
    pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, "ExposureAtInception");
    pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, "ExposureAtAudit");

    pivotTable.AddCalculatedField("ChangeInExp", "=IF(ExposureAtAudit=0,IF(ExposureAtInception=0,0,-1),IF(ExposureAtInception=0,1,(ExposureAtAudit-ExposureAtInception)/ExposureAtInception))");

    pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, "WrittenPremiumAtInception");
    pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, "WrittenPremiumAllEndorsements");
    pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, "PremiumAtAudit");

    pivotTable.AddCalculatedField("ChangeInPrem", "=IF(PremiumAtAudit=0,IF(WrittenPremiumAtInception=0,0,-1),IF(WrittenPremiumAtInception=0,IF(PremiumAtAudit<0,(PremiumAtAudit/PremiumAtAudit)*-1,(PremiumAtAudit/PremiumAtAudit)),(PremiumAtAudit-WrittenPremiumAtInception)/WrittenPremiumAtInception))");

    pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Column, pivotTable.DataField);

    //Update Captions and NumberFormats
    pivotDataFields = pivotTable.DataFields;

    pivotDataFields["ExposureAtInception"].DisplayName = "Exposure At Inception";
    pivotDataFields["ExposureAtInception"].NumberFormat = "$#,##0.00_);[Red]($#,##0.00)";

    pivotDataFields["ExposureAtAudit"].DisplayName = "Exposure At Audit";
    pivotDataFields["ExposureAtAudit"].NumberFormat = "$#,##0.00_);[Red]($#,##0.00)";

    pivotDataFields["ChangeInExp"].DisplayName = "Change In Exp";
    pivotDataFields["ChangeInExp"].NumberFormat = "0.0%;[Red](0.0%)";

    pivotDataFields["WrittenPremiumAtInception"].DisplayName = "Premium At Inception";
    pivotDataFields["WrittenPremiumAtInception"].NumberFormat = "$#,##0.00_);[Red]($#,##0.00)";

    pivotDataFields["WrittenPremiumAllEndorsements"].DisplayName = "Premium All Endorsements";
    pivotDataFields["WrittenPremiumAllEndorsements"].NumberFormat = "$#,##0.00_);[Red]($#,##0.00)";

    pivotDataFields["PremiumAtAudit"].DisplayName = "Premium At Audit";
    pivotDataFields["PremiumAtAudit"].NumberFormat = "$#,##0.00_);[Red]($#,##0.00)";

    pivotDataFields["ChangeInPrem"].DisplayName = "Change In Prem";
    pivotDataFields["ChangeInPrem"].NumberFormat = "0.0%;[Red](0.0%)";


    pivotTable.FormatAll(style);

    //pivotTable.IsGridDropZones = true;
    pivotTable.RefreshData();
    pivotTable.CalculateData();
    pivotTable.RefreshDataOnOpeningFile = true;

    //Autofit all columns and rows
    worksheet.AutoFitColumns();
    worksheet.AutoFitRows();

    Console.WriteLine("{0} End GL Audit Summary pivot", DateTime.Now.ToString());

    // End GL Audit Summary Pivot Table


    // Begin GL Audit Totals Pivot Table

    Console.WriteLine("{0} Begin GL Audit Totals pivot", DateTime.Now.ToString());

    worksheet = workbook.Worksheets.Add("GL Audit Totals");
    worksheet.MoveTo(workbook.Worksheets["GL Audit Summary"].Index + 1);

    detailWorksheet = workbook.Worksheets["GL Audit Detail"];

    pivotTables = worksheet.PivotTables;

    pivotTableIndex = pivotTables.Add(string.Format("'GL Audit Detail'!A1:{0}", CellsHelper.CellIndexToName(detailWorksheet.Cells.MaxDataRow, 30)), "A1", "PivotTable2");

    pivotTable = pivotTables[pivotTableIndex];


    //RowFields
    pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, "ProgramName");

    //Uncheck "(blank)" item
    pivotField = pivotTable.RowFields["ProgramName"];
    pivotField.IsAutoSort = true;
    pivotField.IsAscendSort = true;

    pivotItems = pivotField.PivotItems;

    if (pivotItems.Count > 1)
    {

        for (int i = 0; i < pivotItems.Count; i++)
        {
            pivotItem = pivotItems[i];
            if (pivotItem.Name != null)
            {
                if (pivotItem.Name.Equals("(blank)"))
                {
                    pivotItem.IsHidden = true;
                }
            }
        }
    }


    //DataFields
    pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, "ExposureAtInception");
    pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, "ExposureAtAudit");

    /*
        THE CODE IS FAILING ON THE FOLLOWING LINE

        From what I can tell, it is due to me re-using the exact same cell range from the previous pivot table

        pivotTableIndex = pivotTables.Add(string.Format("'GL Audit Detail'!A1:{0}", CellsHelper.CellIndexToName(detailWorksheet.Cells.MaxDataRow, 30)), "A1", "PivotTable2");

        If I change the column 30 to something else, like 31, the following line of code does not generate the error
    */
    pivotTable.AddCalculatedField("ChangeInExp", "=IF(ExposureAtAudit=0,IF(ExposureAtInception=0,0,-1),IF(ExposureAtInception=0,1,(ExposureAtAudit-ExposureAtInception)/ExposureAtInception))");

    pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, "WrittenPremiumAtInception");
    pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, "WrittenPremiumAllEndorsements");
    pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, "PremiumAtAudit");

    pivotTable.AddCalculatedField("ChangeInPrem", "=IF(PremiumAtAudit=0,IF(WrittenPremiumAtInception=0,0,-1),IF(WrittenPremiumAtInception=0,IF(PremiumAtAudit<0,(PremiumAtAudit/PremiumAtAudit)*-1,(PremiumAtAudit/PremiumAtAudit)),(PremiumAtAudit-WrittenPremiumAtInception)/WrittenPremiumAtInception))");


    //Update Captions and NumberFormats
    pivotDataFields = pivotTable.DataFields;

    pivotDataFields["ExposureAtInception"].DisplayName = "Exposure At Inception";
    pivotDataFields["ExposureAtInception"].NumberFormat = "$#,##0.00_);[Red]($#,##0.00)";

    pivotDataFields["ExposureAtAudit"].DisplayName = "Exposure At Audit";
    pivotDataFields["ExposureAtAudit"].NumberFormat = "$#,##0.00_);[Red]($#,##0.00)";

    pivotDataFields["ChangeInExp"].DisplayName = "Change In Exp";
    pivotDataFields["ChangeInExp"].NumberFormat = "0.0%;[Red](0.0%)";

    pivotDataFields["WrittenPremiumAtInception"].DisplayName = "Premium At Inception";
    pivotDataFields["WrittenPremiumAtInception"].NumberFormat = "$#,##0.00_);[Red]($#,##0.00)";

    pivotDataFields["WrittenPremiumAllEndorsements"].DisplayName = "Premium All Endorsements";
    pivotDataFields["WrittenPremiumAllEndorsements"].NumberFormat = "$#,##0.00_);[Red]($#,##0.00)";

    pivotDataFields["PremiumAtAudit"].DisplayName = "Premium At Audit";
    pivotDataFields["PremiumAtAudit"].NumberFormat = "$#,##0.00_);[Red]($#,##0.00)";

    pivotDataFields["ChangeInPrem"].DisplayName = "Change In Prem";
    pivotDataFields["ChangeInPrem"].NumberFormat = "0.0%;[Red](0.0%)";


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

    Console.WriteLine("{0} End GL Audit Totals pivot", DateTime.Now.ToString());

    // End GL Audit Totals Pivot Table


    // Begin GL Audit History Summary Pivot Table

    Console.WriteLine("{0} Begin GL Audit History Summary pivot", DateTime.Now.ToString());

    detailWorksheet = workbook.Worksheets["GL Audit History Detail"];

    worksheet = workbook.Worksheets.Add("GL Audit History Summary");
    worksheet.MoveTo(workbook.Worksheets["GL Audit Totals"].Index + 1);

    pivotTables = worksheet.PivotTables;

    pivotTableIndex = pivotTables.Add(string.Format("'GL Audit History Detail'!A1:{0}", CellsHelper.CellIndexToName(detailWorksheet.Cells.MaxDataRow, 30)), "A1", "PivotTable3");

    pivotTable = pivotTables[pivotTableIndex];

    pivotTable.PivotTableStyleType = Aspose.Cells.Pivot.PivotTableStyleType.PivotTableStyleLight16;

    pivotTable.ShowValuesRow = false;

    //Remove Grand Total
    pivotTable.ShowRowGrandTotals = false;


    //RowFields
    pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, "ProgramName");

    //Uncheck "(blank)" item
    pivotField = pivotTable.RowFields["ProgramName"];
    pivotField.IsAutoSort = true;
    pivotField.IsAscendSort = true;
    pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

    pivotItems = pivotField.PivotItems;

    if (pivotItems.Count > 1)
    {

        for (int i = 0; i < pivotItems.Count; i++)
        {
            pivotItem = pivotItems[i];
            if (pivotItem.Name != null)
            {
                if (pivotItem.Name.Equals("(blank)"))
                {
                    pivotItem.IsHidden = true;
                }
            }
        }
    }

    pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, "PolicyNumber");
    //Hide Subtotal
    pivotField = pivotTable.RowFields["PolicyNumber"];
    pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

    pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, "InsuredName");
    //Hide Subtotal
    pivotField = pivotTable.RowFields["InsuredName"];
    pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

    pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, "EffDate");
    //Hide Subtotal
    pivotField = pivotTable.RowFields["EffDate"];
    pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

    pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, "ExpDate");
    //Hide Subtotal
    pivotField = pivotTable.RowFields["ExpDate"];
    pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

    pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, "RiskState");
    //Hide Subtotal
    pivotField = pivotTable.RowFields["RiskState"];
    pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

    pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, "ExpBasis");
    //Hide Subtotal
    pivotField = pivotTable.RowFields["ExpBasis"];
    pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

    pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, "FirstAuditRevNumber");
    //Hide Subtotal
    pivotField = pivotTable.RowFields["FirstAuditRevNumber"];
    pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

    pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, "FirstAuditAgingDays");
    //Hide Subtotal
    pivotField = pivotTable.RowFields["FirstAuditAgingDays"];
    pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

    pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, "SecondAuditRevNumber");
    //Hide Subtotal
    pivotField = pivotTable.RowFields["SecondAuditRevNumber"];
    pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

    pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, "SecondAuditAgingDays");
    //Hide Subtotal
    pivotField = pivotTable.RowFields["SecondAuditAgingDays"];
    pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

    pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, "ThirdAuditRevNumber");
    //Hide Subtotal
    pivotField = pivotTable.RowFields["ThirdAuditRevNumber"];
    pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

    pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, "ThirdAuditAgingDays");
    //Hide Subtotal
    pivotField = pivotTable.RowFields["ThirdAuditAgingDays"];
    pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);


    //DataFields
    pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, "ExposureAtInception");
    pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, "ExposureAtAudit");

    pivotTable.AddCalculatedField("ChangeInExp", "=IF(ExposureAtAudit=0,IF(ExposureAtInception=0,0,-1),IF(ExposureAtInception=0,1,(ExposureAtAudit-ExposureAtInception)/ExposureAtInception))");

    pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, "WrittenPremiumAtInception");
    pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, "WrittenPremiumAllEndorsements");
    pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, "PremiumAtAudit");

    pivotTable.AddCalculatedField("ChangeInPrem", "=IF(PremiumAtAudit=0,IF(WrittenPremiumAtInception=0,0,-1),IF(WrittenPremiumAtInception=0,IF(PremiumAtAudit<0,(PremiumAtAudit/PremiumAtAudit)*-1,(PremiumAtAudit/PremiumAtAudit)),(PremiumAtAudit-WrittenPremiumAtInception)/WrittenPremiumAtInception))");

    pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Column, pivotTable.DataField);

    //Update Captions and NumberFormats
    pivotDataFields = pivotTable.DataFields;

    pivotDataFields["ExposureAtInception"].DisplayName = "Exposure At Inception";
    pivotDataFields["ExposureAtInception"].NumberFormat = "$#,##0.00_);[Red]($#,##0.00)";

    pivotDataFields["ExposureAtAudit"].DisplayName = "Exposure At Audit";
    pivotDataFields["ExposureAtAudit"].NumberFormat = "$#,##0.00_);[Red]($#,##0.00)";

    pivotDataFields["ChangeInExp"].DisplayName = "Change In Exp";
    pivotDataFields["ChangeInExp"].NumberFormat = "0.0%;[Red](0.0%)";

    pivotDataFields["WrittenPremiumAtInception"].DisplayName = "Premium At Inception";
    pivotDataFields["WrittenPremiumAtInception"].NumberFormat = "$#,##0.00_);[Red]($#,##0.00)";

    pivotDataFields["WrittenPremiumAllEndorsements"].DisplayName = "Premium All Endorsements";
    pivotDataFields["WrittenPremiumAllEndorsements"].NumberFormat = "$#,##0.00_);[Red]($#,##0.00)";

    pivotDataFields["PremiumAtAudit"].DisplayName = "Premium At Audit";
    pivotDataFields["PremiumAtAudit"].NumberFormat = "$#,##0.00_);[Red]($#,##0.00)";

    pivotDataFields["ChangeInPrem"].DisplayName = "Change In Prem";
    pivotDataFields["ChangeInPrem"].NumberFormat = "0.0%;[Red](0.0%)";


    pivotTable.FormatAll(style);

    //pivotTable.IsGridDropZones = true;

    pivotTable.RefreshData();
    pivotTable.CalculateData();
    pivotTable.RefreshDataOnOpeningFile = true;

    //Autofit all columns and rows
    worksheet.AutoFitColumns();
    worksheet.AutoFitRows();

    Console.WriteLine("{0} End GL Audit History Summary pivot", DateTime.Now.ToString());

    // End GL Audit History Summary Pivot Table


    // Begin GL Audit History Totals Pivot Table

    Console.WriteLine("{0} Begin GL Audit History Totals pivot", DateTime.Now.ToString());

    detailWorksheet = workbook.Worksheets["GL Audit History Detail"];

    worksheet = workbook.Worksheets.Add("GL Audit History Totals");
    worksheet.MoveTo(workbook.Worksheets["GL Audit History Summary"].Index + 1);

    pivotTables = worksheet.PivotTables;

    pivotTableIndex = pivotTables.Add(string.Format("'GL Audit History Detail'!A1:{0}", CellsHelper.CellIndexToName(detailWorksheet.Cells.MaxDataRow, 30)), "A1", "PivotTable4");

    pivotTable = pivotTables[pivotTableIndex];

    pivotTable.PivotTableStyleType = Aspose.Cells.Pivot.PivotTableStyleType.PivotTableStyleLight16;

    pivotTable.ShowValuesRow = false;

    //Remove Grand Total
    pivotTable.ShowRowGrandTotals = false;

    //RowFields
    pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, "ProgramName");

    //Uncheck "(blank)" item
    pivotField = pivotTable.RowFields["ProgramName"];
    pivotField.IsAutoSort = true;
    pivotField.IsAscendSort = true;
    pivotField.SetSubtotals(Aspose.Cells.Pivot.PivotFieldSubtotalType.Automatic, false);

    pivotItems = pivotField.PivotItems;

    if (pivotItems.Count > 1)
    {

        for (int i = 0; i < pivotItems.Count; i++)
        {
            pivotItem = pivotItems[i];
            if (pivotItem.Name != null)
            {
                if (pivotItem.Name.Equals("(blank)"))
                {
                    pivotItem.IsHidden = true;
                }
            }
        }
    }


    //DataFields
    pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, "ExposureAtInception");
    pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, "ExposureAtAudit");

    pivotTable.AddCalculatedField("ChangeInExp", "=IF(ExposureAtAudit=0,IF(ExposureAtInception=0,0,-1),IF(ExposureAtInception=0,1,(ExposureAtAudit-ExposureAtInception)/ExposureAtInception))");

    pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, "WrittenPremiumAtInception");
    pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, "WrittenPremiumAllEndorsements");
    pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, "PremiumAtAudit");

    pivotTable.AddCalculatedField("ChangeInPrem", "=IF(PremiumAtAudit=0,IF(WrittenPremiumAtInception=0,0,-1),IF(WrittenPremiumAtInception=0,IF(PremiumAtAudit<0,(PremiumAtAudit/PremiumAtAudit)*-1,(PremiumAtAudit/PremiumAtAudit)),(PremiumAtAudit-WrittenPremiumAtInception)/WrittenPremiumAtInception))");

    pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Column, pivotTable.DataField);

    //Update Captions and NumberFormats
    pivotDataFields = pivotTable.DataFields;

    pivotDataFields["ExposureAtInception"].DisplayName = "Exposure At Inception";
    pivotDataFields["ExposureAtInception"].NumberFormat = "$#,##0.00_);[Red]($#,##0.00)";

    pivotDataFields["ExposureAtAudit"].DisplayName = "Exposure At Audit";
    pivotDataFields["ExposureAtAudit"].NumberFormat = "$#,##0.00_);[Red]($#,##0.00)";

    pivotDataFields["ChangeInExp"].DisplayName = "Change In Exp";
    pivotDataFields["ChangeInExp"].NumberFormat = "0.0%;[Red](0.0%)";

    pivotDataFields["WrittenPremiumAtInception"].DisplayName = "Premium At Inception";
    pivotDataFields["WrittenPremiumAtInception"].NumberFormat = "$#,##0.00_);[Red]($#,##0.00)";

    pivotDataFields["WrittenPremiumAllEndorsements"].DisplayName = "Premium All Endorsements";
    pivotDataFields["WrittenPremiumAllEndorsements"].NumberFormat = "$#,##0.00_);[Red]($#,##0.00)";

    pivotDataFields["PremiumAtAudit"].DisplayName = "Premium At Audit";
    pivotDataFields["PremiumAtAudit"].NumberFormat = "$#,##0.00_);[Red]($#,##0.00)";

    pivotDataFields["ChangeInPrem"].DisplayName = "Change In Prem";
    pivotDataFields["ChangeInPrem"].NumberFormat = "0.0%;[Red](0.0%)";


    pivotTable.FormatAll(style);

    //pivotTable.IsGridDropZones = true;

           
    pivotTable.RefreshData();
    pivotTable.CalculateData();
          
    pivotTable.RefreshDataOnOpeningFile = true;

    //Autofit all columns and rows
    worksheet.AutoFitColumns();
    worksheet.AutoFitRows();

    Console.WriteLine("{0} End GL Audit History Totals pivot", DateTime.Now.ToString());

    workbook.Save(outFilePath);
}
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


