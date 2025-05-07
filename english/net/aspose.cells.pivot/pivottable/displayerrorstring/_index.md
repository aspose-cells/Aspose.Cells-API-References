---
title: PivotTable.DisplayErrorString
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Indicates whether the PivotTable report displays a custom string in cells that contain errors
type: docs
url: /net/aspose.cells.pivot/pivottable/displayerrorstring/
---
## PivotTable.DisplayErrorString property

Indicates whether the PivotTable report displays a custom string in cells that contain errors.

```csharp
public bool DisplayErrorString { get; set; }
```

### Examples

```csharp
// Called: obj.Worksheets["BP"].PivotTables[0].DisplayErrorString = true;
[Test]
         public void Property_DisplayErrorString()
         {
             Console.WriteLine("testCELLSNET_40010()");
             string infn = path + @"CELLSNET-40010\Multi-level+Category.xlsx";
             string outfn = destpath + @"Multi-level+Category.out.xlsx";

             string connString = "Provider=Microsoft.ACE.OLEDB.12.0;Data Source=" + infn + ";Extended Properties=Excel 12.0"; // for xlsx
             OleDbConnection oledbConn = new OleDbConnection(connString);
             DataSet ds = new DataSet();
             try
             {
                 oledbConn.Open();
                 OleDbCommand cmd = new OleDbCommand("SELECT * FROM [Sheet1$]", oledbConn);
                 OleDbDataAdapter oleda = new OleDbDataAdapter();
                 oleda.SelectCommand = cmd;
                 oleda.Fill(ds);
             }
             catch(Exception e)
             {
                 Console.WriteLine(e.Message);
                 Console.WriteLine("Stop this test case because loading data source failed.");
                 return;
             }
             finally
             {
                 oledbConn.Close();
             }
             Workbook obj = new Workbook();

             DataTable dtDetails = ds.Tables[0];
             string dateFormat = "DD/MM/YYYY HH:MM:SS";
             string dateFormatTime = "[hh]:mm";

             string[] sheetname = new string[4];
             sheetname[0] = "DATA";
             sheetname[1] = "VSummary";
             sheetname[2] = "PSummary";
             sheetname[3] = "BP";

             if (dtDetails.Rows.Count > 0)
             {
                 PivotExcel.CreateEmptySheets(obj, false, sheetname);
                 obj.Worksheets[0].IsGridlinesVisible = true;
                 PivotExcel.CreateDataSheet(obj, 0, dtDetails, true, 8, 1, false, false, true);
                 obj.Worksheets[0].AutoFilter.Range = "A8:AG8";
                 obj.ChangePalette(Color.Firebrick, 55);
                 obj.ChangePalette(Color.FromArgb(153, 204, 255), 54);

                 obj.Worksheets["DATA"].Cells.SetRowHeight(7, 35);

                 PivotExcel.SetMinmumColumnWidth(obj, 0, 15, 3, 4, 5, 6, 8, 10, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23);
                 PivotExcel.SetMinmumColumnWidth(obj, 0, 12, 1, 2, 7, 9, 11, 12, 28, 29, 30, 31, 32, 33);

                 Aspose.Cells.Style HeaderStyle = obj.CreateStyle();
                HeaderStyle.VerticalAlignment = TextAlignmentType.Top;
                 HeaderStyle.IsTextWrapped = true;
                 HeaderStyle.Font.IsBold = true;
                 HeaderStyle.Font.Size = 8;
                 HeaderStyle.Font.Name = "Arial";
                 HeaderStyle.Font.Color = Color.Maroon;
                 HeaderStyle.ForegroundColor = Color.FromArgb(150, 150, 150);
                 HeaderStyle.Pattern = BackgroundType.Solid;
                 HeaderStyle.BackgroundColor = Color.FromArgb(150, 150, 150);
                 HeaderStyle.Borders[BorderType.TopBorder].Color = Color.Black;
                 HeaderStyle.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
                 HeaderStyle.Borders[BorderType.BottomBorder].Color = Color.Black;
                 HeaderStyle.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
                 HeaderStyle.Borders[BorderType.LeftBorder].Color = Color.Black;
                 HeaderStyle.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
                 HeaderStyle.Borders[BorderType.RightBorder].Color = Color.Black;
                 HeaderStyle.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
                 HeaderStyle.HorizontalAlignment = TextAlignmentType.Left;
                 obj.Worksheets["DATA"].Cells["A8"].SetStyle(HeaderStyle);
                 obj.Worksheets["DATA"].Cells["B8"].SetStyle(HeaderStyle);
                 obj.Worksheets["DATA"].Cells["C8"].SetStyle(HeaderStyle);
                 obj.Worksheets["DATA"].Cells["D8"].SetStyle(HeaderStyle);
                 obj.Worksheets["DATA"].Cells["E8"].SetStyle(HeaderStyle);
                 obj.Worksheets["DATA"].Cells["F8"].SetStyle(HeaderStyle);
                 obj.Worksheets["DATA"].Cells["G8"].SetStyle(HeaderStyle);
                 obj.Worksheets["DATA"].Cells["H8"].SetStyle(HeaderStyle);
                 obj.Worksheets["DATA"].Cells["I8"].SetStyle(HeaderStyle);
                 obj.Worksheets["DATA"].Cells["J8"].SetStyle(HeaderStyle);
                 obj.Worksheets["DATA"].Cells["K8"].SetStyle(HeaderStyle);
                 obj.Worksheets["DATA"].Cells["L8"].SetStyle(HeaderStyle);
                 obj.Worksheets["DATA"].Cells["M8"].SetStyle(HeaderStyle);
                 obj.Worksheets["DATA"].Cells["N8"].SetStyle(HeaderStyle);
                 obj.Worksheets["DATA"].Cells["O8"].SetStyle(HeaderStyle);
                 obj.Worksheets["DATA"].Cells["P8"].SetStyle(HeaderStyle);
                 obj.Worksheets["DATA"].Cells["Q8"].SetStyle(HeaderStyle);
                 obj.Worksheets["DATA"].Cells["R8"].SetStyle(HeaderStyle);
                 obj.Worksheets["DATA"].Cells["S8"].SetStyle(HeaderStyle);
                 obj.Worksheets["DATA"].Cells["T8"].SetStyle(HeaderStyle);
                 obj.Worksheets["DATA"].Cells["U8"].SetStyle(HeaderStyle);
                 obj.Worksheets["DATA"].Cells["W8"].SetStyle(HeaderStyle);
                 obj.Worksheets["DATA"].Cells["X8"].SetStyle(HeaderStyle);
                 obj.Worksheets["DATA"].Cells["Y8"].SetStyle(HeaderStyle);
                 obj.Worksheets["DATA"].Cells["Z8"].SetStyle(HeaderStyle);
                 obj.Worksheets["DATA"].Cells["AA8"].SetStyle(HeaderStyle);
                 obj.Worksheets["DATA"].Cells["AB8"].SetStyle(HeaderStyle);
                 obj.Worksheets["DATA"].Cells["AC8"].SetStyle(HeaderStyle);
                 obj.Worksheets["DATA"].Cells["AD8"].SetStyle(HeaderStyle);
                 obj.Worksheets["DATA"].Cells["AE8"].SetStyle(HeaderStyle);
                 obj.Worksheets["DATA"].Cells["AF8"].SetStyle(HeaderStyle);
                 obj.Worksheets["DATA"].Cells["AG8"].SetStyle(HeaderStyle);
                 HeaderStyle.ForegroundColor = Color.FromArgb(230, 184, 183);
                 obj.Worksheets["DATA"].Cells["V8"].SetStyle(HeaderStyle);

                 PivotExcel.SetAreaCellBorder(obj, 0, 8, 0, dtDetails.Rows.Count, 33, CellBorderType.Thin, CellBorderType.Thin, CellBorderType.Thin, CellBorderType.Thin, Color.White, Color.Black);
                 PivotExcel.SetAreaFontFormat(obj, 0, 9, 1, dtDetails.Rows.Count, 33, "Arial", 8, false, false, FontUnderlineType.None, Color.Black, false);

                 int startIdx = 9;
                 int rowCount = 0;
                 Aspose.Cells.Style objStyle = obj.CreateStyle();
                objStyle.Custom = dateFormat;
                 objStyle.Font.Name = "Arial";
                 objStyle.Font.Size = 8;
                 objStyle.Borders[BorderType.TopBorder].Color = Color.Black;
                 objStyle.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
                 objStyle.Borders[BorderType.BottomBorder].Color = Color.Black;
                 objStyle.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
                 objStyle.Borders[BorderType.LeftBorder].Color = Color.Black;
                 objStyle.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
                 objStyle.Borders[BorderType.RightBorder].Color = Color.Black;
                 objStyle.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;

                 Aspose.Cells.Style objStyleTime = obj.CreateStyle();
                objStyleTime.Custom = dateFormatTime;
                 objStyleTime.Font.Name = "Arial";
                 objStyleTime.Font.Size = 8;
                 objStyleTime.HorizontalAlignment = TextAlignmentType.Right;
                 objStyleTime.Borders[BorderType.TopBorder].Color = Color.Black;
                 objStyleTime.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
                 objStyleTime.Borders[BorderType.BottomBorder].Color = Color.Black;
                 objStyleTime.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
                 objStyleTime.Borders[BorderType.LeftBorder].Color = Color.Black;
                 objStyleTime.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
                 objStyleTime.Borders[BorderType.RightBorder].Color = Color.Black;
                 objStyleTime.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
                 objStyleTime.ForegroundColor = Color.FromArgb(217, 217, 217);
                 objStyleTime.Pattern = BackgroundType.Solid;
                 objStyleTime.BackgroundColor = Color.FromArgb(217, 217, 217);

                 Aspose.Cells.Style objStyleColor = obj.CreateStyle();
                objStyleColor.Font.Name = "Arial";
                 objStyleColor.Font.Size = 8;
                 objStyleColor.HorizontalAlignment = TextAlignmentType.Left;
                 objStyleColor.Borders[BorderType.TopBorder].Color = Color.Black;
                 objStyleColor.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
                 objStyleColor.Borders[BorderType.BottomBorder].Color = Color.Black;
                 objStyleColor.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
                 objStyleColor.Borders[BorderType.LeftBorder].Color = Color.Black;
                 objStyleColor.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
                 objStyleColor.Borders[BorderType.RightBorder].Color = Color.Black;
                 objStyleColor.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
                 objStyleColor.ForegroundColor = Color.FromArgb(217, 217, 217);
                 objStyleColor.Pattern = BackgroundType.Solid;
                 objStyleColor.BackgroundColor = Color.FromArgb(217, 217, 217);


                 int CellNo;
                 int CellNoPrevious;
                 String FormulaPortCall = "";
                 String FormulaBerthCall = "";
                 String FormulaTimeatPort = "";
                 String FormulaTimeatBerth = "";
                 String FormulaNORTendered_AllFast = "";
                 String FormulaAllFast_HoseConnected = "";
                 String FormulaHoseConnected_CargoOpsCommence = "";
                 String FormulaCargoOps = "";
                 String FormulaCargoOps_HoseDisconnect = "";
                 String FormulaHoseDisconnected_AllLinesOnDeck = "";

                 foreach (DataRow drDate in dtDetails.Rows)
                 {
                     if (!string.IsNullOrEmpty(drDate["ATA"].ToString()))
                     {
                         obj.Worksheets[0].Cells["N" + (rowCount + startIdx)].PutValue(drDate["ATA"].ToString(), true);
                         obj.Worksheets[0].Cells["N" + (rowCount + startIdx)].SetStyle(objStyle);
                     }
                     else
                     {
                         obj.Worksheets[0].Cells["N" + (rowCount + startIdx)].SetStyle(objStyle);
                     }
                     if (!string.IsNullOrEmpty(drDate["Terminal/Berth - First line ashore"].ToString()))
                     {
                         obj.Worksheets[0].Cells["O" + (rowCount + startIdx)].PutValue(drDate["Terminal/Berth - First line ashore"].ToString(), true);
                         obj.Worksheets[0].Cells["O" + (rowCount + startIdx)].SetStyle(objStyle);
                     }
                     else
                     {
                         obj.Worksheets[0].Cells["O" + (rowCount + startIdx)].SetStyle(objStyle);
                     }
                     if (!string.IsNullOrEmpty(drDate["NOR tendered"].ToString()))
                     {
                         obj.Worksheets[0].Cells["P" + (rowCount + startIdx)].PutValue(drDate["NOR tendered"].ToString(), true);
                         obj.Worksheets[0].Cells["P" + (rowCount + startIdx)].SetStyle(objStyle);
                     }
                     else
                     {
                         obj.Worksheets[0].Cells["P" + (rowCount + startIdx)].SetStyle(objStyle);
                     }

                     if (!string.IsNullOrEmpty(drDate["All fast"].ToString()))
                     {
                         obj.Worksheets[0].Cells["Q" + (rowCount + startIdx)].PutValue(drDate["All fast"].ToString(), true);
                         obj.Worksheets[0].Cells["Q" + (rowCount + startIdx)].SetStyle(objStyle);
                     }
                     else
                     {
                         obj.Worksheets[0].Cells["Q" + (rowCount + startIdx)].SetStyle(objStyle);
                     }

                     if (!string.IsNullOrEmpty(drDate["Hose(s)/Arms connected - Cargo"].ToString()))
                     {
                         obj.Worksheets[0].Cells["R" + (rowCount + startIdx)].PutValue(drDate["Hose(s)/Arms connected - Cargo"].ToString(), true);
                         obj.Worksheets[0].Cells["R" + (rowCount + startIdx)].SetStyle(objStyle);
                     }
                     else
                     {
                         obj.Worksheets[0].Cells["R" + (rowCount + startIdx)].SetStyle(objStyle);

                     }

                     if (!string.IsNullOrEmpty(drDate["Commenced Ops"].ToString()))
                     {
                         obj.Worksheets[0].Cells["S" + (rowCount + startIdx)].PutValue(drDate["Commenced Ops"].ToString(), true);
                         obj.Worksheets[0].Cells["S" + (rowCount + startIdx)].SetStyle(objStyle);
                     }
                     else
                     {
                         obj.Worksheets[0].Cells["S" + (rowCount + startIdx)].SetStyle(objStyle);

                     }

                     if (!string.IsNullOrEmpty(drDate["Completed ops"].ToString()))
                     {
                         obj.Worksheets[0].Cells["T" + (rowCount + startIdx)].PutValue(drDate["Completed ops"].ToString(), true);
                         obj.Worksheets[0].Cells["T" + (rowCount + startIdx)].SetStyle(objStyle);
                     }
                     else
                     {
                         obj.Worksheets[0].Cells["T" + (rowCount + startIdx)].SetStyle(objStyle);
                     }

                     if (!string.IsNullOrEmpty(drDate["Hose(s)/arms disconnected - Cargo"].ToString()))
                     {
                         obj.Worksheets[0].Cells["U" + (rowCount + startIdx)].PutValue(drDate["Hose(s)/arms disconnected - Cargo"].ToString(), true);
                         obj.Worksheets[0].Cells["U" + (rowCount + startIdx)].SetStyle(objStyle);
                     }
                     else
                     {
                         obj.Worksheets[0].Cells["U" + (rowCount + startIdx)].SetStyle(objStyle);
                     }
                     if (!string.IsNullOrEmpty(drDate["All lines on deck"].ToString()))
                     {
                         obj.Worksheets[0].Cells["V" + (rowCount + startIdx)].PutValue(drDate["All lines on deck"].ToString(), true);
                         obj.Worksheets[0].Cells["V" + (rowCount + startIdx)].SetStyle(objStyle);
                     }
                     else
                     {
                         obj.Worksheets[0].Cells["V" + (rowCount + startIdx)].SetStyle(objStyle);
                     }
                     if (!string.IsNullOrEmpty(drDate["ATS"].ToString()))
                     {
                         obj.Worksheets[0].Cells["W" + (rowCount + startIdx)].PutValue(drDate["ATS"].ToString(), true);
                         obj.Worksheets[0].Cells["W" + (rowCount + startIdx)].SetStyle(objStyle);
                     }
                     else
                     {
                         obj.Worksheets[0].Cells["W" + (rowCount + startIdx)].SetStyle(objStyle);
                     }

                     CellNo = rowCount + startIdx;
                     CellNoPrevious = rowCount + startIdx - 1;

                     FormulaPortCall = "=IF((C" + CellNo.ToString() + @"=C" + CellNoPrevious.ToString() + @")=FALSE,""Yes"",""No"")";
                     obj.Worksheets[0].Cells["X" + (rowCount + startIdx)].Formula = FormulaPortCall;
                     obj.Worksheets[0].Cells["X" + (rowCount + startIdx)].SetStyle(objStyleColor);

                     FormulaTimeatPort = "=IF(OR(W" + CellNo.ToString() + @"="""",N" + CellNo.ToString() + @"=""""),"""",IF(W" + CellNo.ToString() + ">N" + CellNo.ToString() + ",W" + CellNo.ToString() + "-N" + CellNo.ToString() + @",""""))";
                     obj.Worksheets[0].Cells["Y" + (rowCount + startIdx)].Formula = FormulaTimeatPort;
                     obj.Worksheets[0].Cells["Y" + (rowCount + startIdx)].SetStyle(objStyleTime);

                     FormulaBerthCall = "=IF(X" + CellNo.ToString() + @"=""Yes"",""Yes"",IF((H" + CellNo.ToString() + @"=H" + CellNoPrevious.ToString() + @")=FALSE,""Yes"",""No""))";
                     obj.Worksheets[0].Cells["Z" + (rowCount + startIdx)].Formula = FormulaBerthCall;
                     obj.Worksheets[0].Cells["Z" + (rowCount + startIdx)].SetStyle(objStyleColor);

                     FormulaTimeatBerth = "=IF(OR(V" + CellNo.ToString() + @"="""",O" + CellNo.ToString() + @"=""""),"""",IF(V" + CellNo.ToString() + ">O" + CellNo.ToString() + ",V" + CellNo.ToString() + "-O" + CellNo.ToString() + @",""""))";
                     obj.Worksheets[0].Cells["AA" + (rowCount + startIdx)].Formula = FormulaTimeatBerth;
                     obj.Worksheets[0].Cells["AA" + (rowCount + startIdx)].SetStyle(objStyleTime);

                     FormulaNORTendered_AllFast = "=IF(OR(Q" + CellNo.ToString() + @"="""",P" + CellNo.ToString() + @"=""""),"""",IF((Q" + CellNo.ToString() + "-P" + CellNo.ToString() + ")>0,Q" + CellNo.ToString() + "-P" + CellNo.ToString() + @",0))";
                     obj.Worksheets[0].Cells["AB" + (rowCount + startIdx)].Formula = FormulaNORTendered_AllFast;
                     obj.Worksheets[0].Cells["AB" + (rowCount + startIdx)].SetStyle(objStyleTime);

                     FormulaAllFast_HoseConnected = "=IF(OR(R" + CellNo.ToString() + @"="""",Q" + CellNo.ToString() + @"=""""),"""",IF((R" + CellNo.ToString() + "-Q" + CellNo.ToString() + ")>0,R" + CellNo.ToString() + "-Q" + CellNo.ToString() + @",0))";
                     obj.Worksheets[0].Cells["AC" + (rowCount + startIdx)].Formula = FormulaAllFast_HoseConnected;
                     obj.Worksheets[0].Cells["AC" + (rowCount + startIdx)].SetStyle(objStyleTime);

                     FormulaHoseConnected_CargoOpsCommence = "=IF(OR(S" + CellNo.ToString() + @"="""",R" + CellNo.ToString() + @"=""""),"""",IF((S" + CellNo.ToString() + "-R" + CellNo.ToString() + ")>0,S" + CellNo.ToString() + "-R" + CellNo.ToString() + @",0))";
                     obj.Worksheets[0].Cells["AD" + (rowCount + startIdx)].Formula = FormulaHoseConnected_CargoOpsCommence;
                     obj.Worksheets[0].Cells["AD" + (rowCount + startIdx)].SetStyle(objStyleTime);

                     FormulaCargoOps = "=IF(OR(T" + CellNo.ToString() + @"="""",S" + CellNo.ToString() + @"=""""),"""",IF((T" + CellNo.ToString() + "-S" + CellNo.ToString() + ")>0,T" + CellNo.ToString() + "-S" + CellNo.ToString() + @",0))";
                     obj.Worksheets[0].Cells["AE" + (rowCount + startIdx)].Formula = FormulaCargoOps;
                     obj.Worksheets[0].Cells["AE" + (rowCount + startIdx)].SetStyle(objStyleTime);

                     FormulaCargoOps_HoseDisconnect = "=IF(OR(U" + CellNo.ToString() + @"="""",T" + CellNo.ToString() + @"=""""),"""",IF((U" + CellNo.ToString() + "-T" + CellNo.ToString() + ")>0,U" + CellNo.ToString() + "-T" + CellNo.ToString() + @",0))";
                     obj.Worksheets[0].Cells["AF" + (rowCount + startIdx)].Formula = FormulaCargoOps_HoseDisconnect;
                     obj.Worksheets[0].Cells["AF" + (rowCount + startIdx)].SetStyle(objStyleTime);

                     FormulaHoseDisconnected_AllLinesOnDeck = "=IF(OR(V" + CellNo.ToString() + @"="""",U" + CellNo.ToString() + @"=""""),"""",IF((V" + CellNo.ToString() + "-U" + CellNo.ToString() + ")>0,V" + CellNo.ToString() + "-U" + CellNo.ToString() + @",0))";
                     obj.Worksheets[0].Cells["AG" + (rowCount + startIdx)].Formula = FormulaHoseDisconnected_AllLinesOnDeck;
                     obj.Worksheets[0].Cells["AG" + (rowCount + startIdx)].SetStyle(objStyleTime);

                     rowCount++;
                 }

                 // BP

                 try
                 {
                     PivotTableCollection pivotTables = obj.Worksheets["BP"].PivotTables;
                     string pivotDataSourceArea = "DATA!A8:" + obj.Worksheets["DATA"].Cells[dtDetails.Rows.Count + 7, dtDetails.Columns.Count - 1].Name;
                     string startingCell = "A36";
                     string pivotTableName = "PivotTable";
                     int index = pivotTables.Add(pivotDataSourceArea, startingCell, pivotTableName);
                     PivotTable pivotTable = pivotTables[index];

                     pivotTable.RowFields.AddByBaseIndex(dtDetails.Columns["Terminal/Berth - First line ashore"].Ordinal);
                     pivotTable.RowFields.AddByBaseIndex(dtDetails.Columns["PortLog - Terminal/Berth/ETA"].Ordinal);
                     pivotTable.RowFields.AddByBaseIndex(dtDetails.Columns["Cargo Activity"].Ordinal);
                     pivotTable.RowFields.AddByBaseIndex(dtDetails.Columns["PortLog - Cargo No"].Ordinal);
                     pivotTable.RowFields.AddByBaseIndex(dtDetails.Columns["PortLog - Trade Name"].Ordinal);

                     pivotTable.DataFields.AddByBaseIndex(dtDetails.Columns["All Fast"].Ordinal);
                     pivotTable.DataFields.AddByBaseIndex(dtDetails.Columns["All Fast to hose connected"].Ordinal);
                     pivotTable.DataFields.AddByBaseIndex(dtDetails.Columns["Hose connected to cargo ops commence"].Ordinal);
                     pivotTable.DataFields.AddByBaseIndex(dtDetails.Columns["Cargo Ops"].Ordinal);
                     pivotTable.DataFields.AddByBaseIndex(dtDetails.Columns["Cargo Ops to hose disconnect"].Ordinal);
                     pivotTable.DataFields.AddByBaseIndex(dtDetails.Columns["Hose disconnected to all lines on deck"].Ordinal);


                     PivotField pivotDataField1 = pivotTable.DataFields[0];
                     pivotDataField1.Function = ConsolidationFunction.Min;
                     pivotDataField1.NumberFormat = "dd-mmm-yy hh:mm";

                     PivotField pivotDataField2 = pivotTable.DataFields[1];
                     pivotDataField2.Function = ConsolidationFunction.Average;
                     pivotDataField2.NumberFormat = "[hh]:mm";

                     PivotField pivotDataField3 = pivotTable.DataFields[2];
                     pivotDataField3.Function = ConsolidationFunction.Average;
                     pivotDataField3.NumberFormat = "[hh]:mm";

                     PivotField pivotDataField4 = pivotTable.DataFields[3];
                     pivotDataField4.Function = ConsolidationFunction.Average;
                     pivotDataField4.NumberFormat = "[hh]:mm";

                     PivotField pivotDataField5 = pivotTable.DataFields[4];
                     pivotDataField5.Function = ConsolidationFunction.Average;
                     pivotDataField5.NumberFormat = "[hh]:mm";

                     PivotField pivotDataField6 = pivotTable.DataFields[5];
                     pivotDataField6.Function = ConsolidationFunction.Average;
                     pivotDataField6.NumberFormat = "[hh]:mm";

                     pivotTable.AddFieldToArea(PivotFieldType.Column, pivotTable.DataField);
                     pivotTable.ShowColumnGrandTotals = false;


                     Aspose.Cells.Style DataStyle = obj.CreateStyle();

                     DataStyle.Font.Size = 8;
                     DataStyle.Font.Name = "Arial";
                     DataStyle.Font.Color = Color.Black;
                     DataStyle.RotationAngle = 90;

                     pivotTable.AutoFormatType = PivotTableAutoFormatType.Classic;

                     pivotTable.DataFields[0].DisplayName = "All Fast ";
                     pivotTable.DataFields[1].DisplayName = "All fast to hose connected";
                     pivotTable.DataFields[2].DisplayName = "Hose conn - cargo ops commence";
                     pivotTable.DataFields[3].DisplayName = "Cargo Ops";
                     pivotTable.DataFields[4].DisplayName = "Cargo Ops complete - hose disconnect";
                     pivotTable.DataFields[5].DisplayName = "Hose disconnected to all lines on deck";

                     pivotTable.PageFields.AddByBaseIndex(dtDetails.Columns["Vessel Name"].Ordinal);
                     pivotTable.PageFields.AddByBaseIndex(dtDetails.Columns["Cargo details-Voyage No"].Ordinal);
                     pivotTable.PageFields.AddByBaseIndex(dtDetails.Columns["Port Name"].Ordinal);
                     pivotTable.PageFields.AddByBaseIndex(dtDetails.Columns["Terminal"].Ordinal);
                     pivotTable.PageFields.AddByBaseIndex(dtDetails.Columns["Berth"].Ordinal);


                     pivotTable.RowFields[0].IsAutoSort = true;
                     pivotTable.RowFields[1].IsAutoSort = true;
                     pivotTable.RowFields[2].IsAutoSort = true;

                     pivotTable.PageFields[0].IsAutoSort = true;
                     pivotTable.PageFields[1].IsAutoSort = true;
                     pivotTable.PageFields[2].IsAutoSort = true;
                     pivotTable.PageFields[3].IsAutoSort = true;
                     pivotTable.PageFields[4].IsAutoSort = true;

                     obj.Worksheets["BP"].PivotTables[0].RowFields[0].IsAutoSubtotals = false;
                     obj.Worksheets["BP"].PivotTables[0].RowFields[1].IsAutoSubtotals = false;
                     obj.Worksheets["BP"].PivotTables[0].RowFields[2].IsAutoSubtotals = false;
                     obj.Worksheets["BP"].PivotTables[0].RowFields[3].IsAutoSubtotals = false;
                     obj.Worksheets["BP"].PivotTables[0].RowFields[0].ShowInOutlineForm = false;
                     obj.Worksheets["BP"].PivotTables[0].ShowRowHeaderCaption = false;
                     obj.Worksheets["BP"].PivotTables[0].RowFields[0].NumberFormat = "m/d/yyyy h:mm";
                     obj.Worksheets["BP"].PivotTables[0].DisplayErrorString = true;
                     obj.Worksheets["BP"].PivotTables[0].RowFields[0].ShowInOutlineForm = false;
                     obj.Worksheets["BP"].PivotTables[0].ShowRowHeaderCaption = false;

                     obj.Worksheets["BP"].Charts.Add(ChartType.BarStacked, 2, 0, 25, 10);
                     obj.Worksheets["BP"].Charts[0].PivotSource = "BP!PivotTable";
                     obj.Worksheets["BP"].Charts[0].ChartArea.Area.ForegroundColor = Color.White;
                     obj.Worksheets["BP"].Charts[0].PlotArea.Area.ForegroundColor = Color.White;
                     obj.Worksheets["BP"].Charts[0].Title.Text = "";
                     obj.Worksheets["BP"].Charts[0].ShowLegend = true;
                     obj.Worksheets["BP"].Charts[0].Legend.Position = LegendPositionType.Top;
                     obj.Worksheets["BP"].Charts[0].ValueAxis.TickLabels.RotationAngle = 45;
                     obj.Worksheets["BP"].Charts[0].ValueAxis.TickLabels.Font.IsBold = false;
                     obj.Worksheets["BP"].Charts[0].ValueAxis.TickLabelPosition = TickLabelPositionType.NextToAxis;
                     obj.Worksheets["BP"].Charts[0].ValueAxis.MajorTickMark = TickMarkType.Outside;
                     obj.Worksheets["BP"].Charts[0].ValueAxis.MinorTickMark = TickMarkType.None;

                     obj.Worksheets["BP"].Charts[0].CategoryAxis.IsPlotOrderReversed = true;
                     obj.Worksheets["BP"].Charts[0].CategoryAxis.HasMultiLevelLabels = true;
                     obj.Worksheets["BP"].Charts[0].CategoryAxis.MajorTickMark = TickMarkType.Inside;
                     obj.Worksheets["BP"].Charts[0].CategoryAxis.MinorTickMark = TickMarkType.None;
                     obj.Worksheets["BP"].Charts[0].CategoryAxis.TickLabelPosition = TickLabelPositionType.NextToAxis;

                 }
                 catch (Exception ex)
                 {
                     obj.Worksheets["BP"].RemoveAllDrawingObjects();
                     obj.Worksheets["BP"].Cells.ClearContents(0, 0, 2000, 2000);
                     obj.Worksheets["BP"].Cells[0, 0].Value = "No data to create pivot table and pivot chart";// "Exception Occurred";
                 }


             }
             //obj.Save("Output.xlsx", SaveType.OpenInBrowser, FileFormatType.Xlsx, HttpContext.Current.Response);
             obj.Save(outfn, SaveFormat.Xlsx);
#if WTEST
            Process.Start("explorer.exe", string.Format("\"{0}\"", outfn));
#endif
         }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


