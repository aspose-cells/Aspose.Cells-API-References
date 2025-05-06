---
title: PivotTable.ShowRowHeaderCaption
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Indicates whether row header caption is shown in the PivotTable report Indicates whether Display field captions and filter drop downs
type: docs
url: /net/aspose.cells.pivot/pivottable/showrowheadercaption/
---
## PivotTable.ShowRowHeaderCaption property

Indicates whether row header caption is shown in the PivotTable report Indicates whether Display field captions and filter drop downs

```csharp
public bool ShowRowHeaderCaption { get; set; }
```

### Examples

```csharp
// Called: obj.Worksheets[&amp;quot;BP&amp;quot;].PivotTables[0].ShowRowHeaderCaption = false;
[Test]
         public void Property_ShowRowHeaderCaption()
         {
             Console.WriteLine(&quot;testCELLSNET_40010()&quot;);
             string infn = path + @&quot;CELLSNET-40010\Multi-level+Category.xlsx&quot;;
             string outfn = destpath + @&quot;Multi-level+Category.out.xlsx&quot;;

             string connString = &quot;Provider=Microsoft.ACE.OLEDB.12.0;Data Source=&quot; + infn + &quot;;Extended Properties=Excel 12.0&quot;; // for xlsx
             OleDbConnection oledbConn = new OleDbConnection(connString);
             DataSet ds = new DataSet();
             try
             {
                 oledbConn.Open();
                 OleDbCommand cmd = new OleDbCommand(&quot;SELECT * FROM [Sheet1$]&quot;, oledbConn);
                 OleDbDataAdapter oleda = new OleDbDataAdapter();
                 oleda.SelectCommand = cmd;
                 oleda.Fill(ds);
             }
             catch(Exception e)
             {
                 Console.WriteLine(e.Message);
                 Console.WriteLine(&quot;Stop this test case because loading data source failed.&quot;);
                 return;
             }
             finally
             {
                 oledbConn.Close();
             }
             Workbook obj = new Workbook();

             DataTable dtDetails = ds.Tables[0];
             string dateFormat = &quot;DD/MM/YYYY HH:MM:SS&quot;;
             string dateFormatTime = &quot;[hh]:mm&quot;;

             string[] sheetname = new string[4];
             sheetname[0] = &quot;DATA&quot;;
             sheetname[1] = &quot;VSummary&quot;;
             sheetname[2] = &quot;PSummary&quot;;
             sheetname[3] = &quot;BP&quot;;

             if (dtDetails.Rows.Count &gt; 0)
             {
                 PivotExcel.CreateEmptySheets(obj, false, sheetname);
                 obj.Worksheets[0].IsGridlinesVisible = true;
                 PivotExcel.CreateDataSheet(obj, 0, dtDetails, true, 8, 1, false, false, true);
                 obj.Worksheets[0].AutoFilter.Range = &quot;A8:AG8&quot;;
                 obj.ChangePalette(Color.Firebrick, 55);
                 obj.ChangePalette(Color.FromArgb(153, 204, 255), 54);

                 obj.Worksheets[&quot;DATA&quot;].Cells.SetRowHeight(7, 35);

                 PivotExcel.SetMinmumColumnWidth(obj, 0, 15, 3, 4, 5, 6, 8, 10, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23);
                 PivotExcel.SetMinmumColumnWidth(obj, 0, 12, 1, 2, 7, 9, 11, 12, 28, 29, 30, 31, 32, 33);

                 Aspose.Cells.Style HeaderStyle = obj.CreateStyle();
                HeaderStyle.VerticalAlignment = TextAlignmentType.Top;
                 HeaderStyle.IsTextWrapped = true;
                 HeaderStyle.Font.IsBold = true;
                 HeaderStyle.Font.Size = 8;
                 HeaderStyle.Font.Name = &quot;Arial&quot;;
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
                 obj.Worksheets[&quot;DATA&quot;].Cells[&quot;A8&quot;].SetStyle(HeaderStyle);
                 obj.Worksheets[&quot;DATA&quot;].Cells[&quot;B8&quot;].SetStyle(HeaderStyle);
                 obj.Worksheets[&quot;DATA&quot;].Cells[&quot;C8&quot;].SetStyle(HeaderStyle);
                 obj.Worksheets[&quot;DATA&quot;].Cells[&quot;D8&quot;].SetStyle(HeaderStyle);
                 obj.Worksheets[&quot;DATA&quot;].Cells[&quot;E8&quot;].SetStyle(HeaderStyle);
                 obj.Worksheets[&quot;DATA&quot;].Cells[&quot;F8&quot;].SetStyle(HeaderStyle);
                 obj.Worksheets[&quot;DATA&quot;].Cells[&quot;G8&quot;].SetStyle(HeaderStyle);
                 obj.Worksheets[&quot;DATA&quot;].Cells[&quot;H8&quot;].SetStyle(HeaderStyle);
                 obj.Worksheets[&quot;DATA&quot;].Cells[&quot;I8&quot;].SetStyle(HeaderStyle);
                 obj.Worksheets[&quot;DATA&quot;].Cells[&quot;J8&quot;].SetStyle(HeaderStyle);
                 obj.Worksheets[&quot;DATA&quot;].Cells[&quot;K8&quot;].SetStyle(HeaderStyle);
                 obj.Worksheets[&quot;DATA&quot;].Cells[&quot;L8&quot;].SetStyle(HeaderStyle);
                 obj.Worksheets[&quot;DATA&quot;].Cells[&quot;M8&quot;].SetStyle(HeaderStyle);
                 obj.Worksheets[&quot;DATA&quot;].Cells[&quot;N8&quot;].SetStyle(HeaderStyle);
                 obj.Worksheets[&quot;DATA&quot;].Cells[&quot;O8&quot;].SetStyle(HeaderStyle);
                 obj.Worksheets[&quot;DATA&quot;].Cells[&quot;P8&quot;].SetStyle(HeaderStyle);
                 obj.Worksheets[&quot;DATA&quot;].Cells[&quot;Q8&quot;].SetStyle(HeaderStyle);
                 obj.Worksheets[&quot;DATA&quot;].Cells[&quot;R8&quot;].SetStyle(HeaderStyle);
                 obj.Worksheets[&quot;DATA&quot;].Cells[&quot;S8&quot;].SetStyle(HeaderStyle);
                 obj.Worksheets[&quot;DATA&quot;].Cells[&quot;T8&quot;].SetStyle(HeaderStyle);
                 obj.Worksheets[&quot;DATA&quot;].Cells[&quot;U8&quot;].SetStyle(HeaderStyle);
                 obj.Worksheets[&quot;DATA&quot;].Cells[&quot;W8&quot;].SetStyle(HeaderStyle);
                 obj.Worksheets[&quot;DATA&quot;].Cells[&quot;X8&quot;].SetStyle(HeaderStyle);
                 obj.Worksheets[&quot;DATA&quot;].Cells[&quot;Y8&quot;].SetStyle(HeaderStyle);
                 obj.Worksheets[&quot;DATA&quot;].Cells[&quot;Z8&quot;].SetStyle(HeaderStyle);
                 obj.Worksheets[&quot;DATA&quot;].Cells[&quot;AA8&quot;].SetStyle(HeaderStyle);
                 obj.Worksheets[&quot;DATA&quot;].Cells[&quot;AB8&quot;].SetStyle(HeaderStyle);
                 obj.Worksheets[&quot;DATA&quot;].Cells[&quot;AC8&quot;].SetStyle(HeaderStyle);
                 obj.Worksheets[&quot;DATA&quot;].Cells[&quot;AD8&quot;].SetStyle(HeaderStyle);
                 obj.Worksheets[&quot;DATA&quot;].Cells[&quot;AE8&quot;].SetStyle(HeaderStyle);
                 obj.Worksheets[&quot;DATA&quot;].Cells[&quot;AF8&quot;].SetStyle(HeaderStyle);
                 obj.Worksheets[&quot;DATA&quot;].Cells[&quot;AG8&quot;].SetStyle(HeaderStyle);
                 HeaderStyle.ForegroundColor = Color.FromArgb(230, 184, 183);
                 obj.Worksheets[&quot;DATA&quot;].Cells[&quot;V8&quot;].SetStyle(HeaderStyle);

                 PivotExcel.SetAreaCellBorder(obj, 0, 8, 0, dtDetails.Rows.Count, 33, CellBorderType.Thin, CellBorderType.Thin, CellBorderType.Thin, CellBorderType.Thin, Color.White, Color.Black);
                 PivotExcel.SetAreaFontFormat(obj, 0, 9, 1, dtDetails.Rows.Count, 33, &quot;Arial&quot;, 8, false, false, FontUnderlineType.None, Color.Black, false);

                 int startIdx = 9;
                 int rowCount = 0;
                 Aspose.Cells.Style objStyle = obj.CreateStyle();
                objStyle.Custom = dateFormat;
                 objStyle.Font.Name = &quot;Arial&quot;;
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
                 objStyleTime.Font.Name = &quot;Arial&quot;;
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
                objStyleColor.Font.Name = &quot;Arial&quot;;
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
                 String FormulaPortCall = &quot;&quot;;
                 String FormulaBerthCall = &quot;&quot;;
                 String FormulaTimeatPort = &quot;&quot;;
                 String FormulaTimeatBerth = &quot;&quot;;
                 String FormulaNORTendered_AllFast = &quot;&quot;;
                 String FormulaAllFast_HoseConnected = &quot;&quot;;
                 String FormulaHoseConnected_CargoOpsCommence = &quot;&quot;;
                 String FormulaCargoOps = &quot;&quot;;
                 String FormulaCargoOps_HoseDisconnect = &quot;&quot;;
                 String FormulaHoseDisconnected_AllLinesOnDeck = &quot;&quot;;

                 foreach (DataRow drDate in dtDetails.Rows)
                 {
                     if (!string.IsNullOrEmpty(drDate[&quot;ATA&quot;].ToString()))
                     {
                         obj.Worksheets[0].Cells[&quot;N&quot; + (rowCount + startIdx)].PutValue(drDate[&quot;ATA&quot;].ToString(), true);
                         obj.Worksheets[0].Cells[&quot;N&quot; + (rowCount + startIdx)].SetStyle(objStyle);
                     }
                     else
                     {
                         obj.Worksheets[0].Cells[&quot;N&quot; + (rowCount + startIdx)].SetStyle(objStyle);
                     }
                     if (!string.IsNullOrEmpty(drDate[&quot;Terminal/Berth - First line ashore&quot;].ToString()))
                     {
                         obj.Worksheets[0].Cells[&quot;O&quot; + (rowCount + startIdx)].PutValue(drDate[&quot;Terminal/Berth - First line ashore&quot;].ToString(), true);
                         obj.Worksheets[0].Cells[&quot;O&quot; + (rowCount + startIdx)].SetStyle(objStyle);
                     }
                     else
                     {
                         obj.Worksheets[0].Cells[&quot;O&quot; + (rowCount + startIdx)].SetStyle(objStyle);
                     }
                     if (!string.IsNullOrEmpty(drDate[&quot;NOR tendered&quot;].ToString()))
                     {
                         obj.Worksheets[0].Cells[&quot;P&quot; + (rowCount + startIdx)].PutValue(drDate[&quot;NOR tendered&quot;].ToString(), true);
                         obj.Worksheets[0].Cells[&quot;P&quot; + (rowCount + startIdx)].SetStyle(objStyle);
                     }
                     else
                     {
                         obj.Worksheets[0].Cells[&quot;P&quot; + (rowCount + startIdx)].SetStyle(objStyle);
                     }

                     if (!string.IsNullOrEmpty(drDate[&quot;All fast&quot;].ToString()))
                     {
                         obj.Worksheets[0].Cells[&quot;Q&quot; + (rowCount + startIdx)].PutValue(drDate[&quot;All fast&quot;].ToString(), true);
                         obj.Worksheets[0].Cells[&quot;Q&quot; + (rowCount + startIdx)].SetStyle(objStyle);
                     }
                     else
                     {
                         obj.Worksheets[0].Cells[&quot;Q&quot; + (rowCount + startIdx)].SetStyle(objStyle);
                     }

                     if (!string.IsNullOrEmpty(drDate[&quot;Hose(s)/Arms connected - Cargo&quot;].ToString()))
                     {
                         obj.Worksheets[0].Cells[&quot;R&quot; + (rowCount + startIdx)].PutValue(drDate[&quot;Hose(s)/Arms connected - Cargo&quot;].ToString(), true);
                         obj.Worksheets[0].Cells[&quot;R&quot; + (rowCount + startIdx)].SetStyle(objStyle);
                     }
                     else
                     {
                         obj.Worksheets[0].Cells[&quot;R&quot; + (rowCount + startIdx)].SetStyle(objStyle);

                     }

                     if (!string.IsNullOrEmpty(drDate[&quot;Commenced Ops&quot;].ToString()))
                     {
                         obj.Worksheets[0].Cells[&quot;S&quot; + (rowCount + startIdx)].PutValue(drDate[&quot;Commenced Ops&quot;].ToString(), true);
                         obj.Worksheets[0].Cells[&quot;S&quot; + (rowCount + startIdx)].SetStyle(objStyle);
                     }
                     else
                     {
                         obj.Worksheets[0].Cells[&quot;S&quot; + (rowCount + startIdx)].SetStyle(objStyle);

                     }

                     if (!string.IsNullOrEmpty(drDate[&quot;Completed ops&quot;].ToString()))
                     {
                         obj.Worksheets[0].Cells[&quot;T&quot; + (rowCount + startIdx)].PutValue(drDate[&quot;Completed ops&quot;].ToString(), true);
                         obj.Worksheets[0].Cells[&quot;T&quot; + (rowCount + startIdx)].SetStyle(objStyle);
                     }
                     else
                     {
                         obj.Worksheets[0].Cells[&quot;T&quot; + (rowCount + startIdx)].SetStyle(objStyle);
                     }

                     if (!string.IsNullOrEmpty(drDate[&quot;Hose(s)/arms disconnected - Cargo&quot;].ToString()))
                     {
                         obj.Worksheets[0].Cells[&quot;U&quot; + (rowCount + startIdx)].PutValue(drDate[&quot;Hose(s)/arms disconnected - Cargo&quot;].ToString(), true);
                         obj.Worksheets[0].Cells[&quot;U&quot; + (rowCount + startIdx)].SetStyle(objStyle);
                     }
                     else
                     {
                         obj.Worksheets[0].Cells[&quot;U&quot; + (rowCount + startIdx)].SetStyle(objStyle);
                     }
                     if (!string.IsNullOrEmpty(drDate[&quot;All lines on deck&quot;].ToString()))
                     {
                         obj.Worksheets[0].Cells[&quot;V&quot; + (rowCount + startIdx)].PutValue(drDate[&quot;All lines on deck&quot;].ToString(), true);
                         obj.Worksheets[0].Cells[&quot;V&quot; + (rowCount + startIdx)].SetStyle(objStyle);
                     }
                     else
                     {
                         obj.Worksheets[0].Cells[&quot;V&quot; + (rowCount + startIdx)].SetStyle(objStyle);
                     }
                     if (!string.IsNullOrEmpty(drDate[&quot;ATS&quot;].ToString()))
                     {
                         obj.Worksheets[0].Cells[&quot;W&quot; + (rowCount + startIdx)].PutValue(drDate[&quot;ATS&quot;].ToString(), true);
                         obj.Worksheets[0].Cells[&quot;W&quot; + (rowCount + startIdx)].SetStyle(objStyle);
                     }
                     else
                     {
                         obj.Worksheets[0].Cells[&quot;W&quot; + (rowCount + startIdx)].SetStyle(objStyle);
                     }

                     CellNo = rowCount + startIdx;
                     CellNoPrevious = rowCount + startIdx - 1;

                     FormulaPortCall = &quot;=IF((C&quot; + CellNo.ToString() + @&quot;=C&quot; + CellNoPrevious.ToString() + @&quot;)=FALSE,&quot;&quot;Yes&quot;&quot;,&quot;&quot;No&quot;&quot;)&quot;;
                     obj.Worksheets[0].Cells[&quot;X&quot; + (rowCount + startIdx)].Formula = FormulaPortCall;
                     obj.Worksheets[0].Cells[&quot;X&quot; + (rowCount + startIdx)].SetStyle(objStyleColor);

                     FormulaTimeatPort = &quot;=IF(OR(W&quot; + CellNo.ToString() + @&quot;=&quot;&quot;&quot;&quot;,N&quot; + CellNo.ToString() + @&quot;=&quot;&quot;&quot;&quot;),&quot;&quot;&quot;&quot;,IF(W&quot; + CellNo.ToString() + &quot;&gt;N&quot; + CellNo.ToString() + &quot;,W&quot; + CellNo.ToString() + &quot;-N&quot; + CellNo.ToString() + @&quot;,&quot;&quot;&quot;&quot;))&quot;;
                     obj.Worksheets[0].Cells[&quot;Y&quot; + (rowCount + startIdx)].Formula = FormulaTimeatPort;
                     obj.Worksheets[0].Cells[&quot;Y&quot; + (rowCount + startIdx)].SetStyle(objStyleTime);

                     FormulaBerthCall = &quot;=IF(X&quot; + CellNo.ToString() + @&quot;=&quot;&quot;Yes&quot;&quot;,&quot;&quot;Yes&quot;&quot;,IF((H&quot; + CellNo.ToString() + @&quot;=H&quot; + CellNoPrevious.ToString() + @&quot;)=FALSE,&quot;&quot;Yes&quot;&quot;,&quot;&quot;No&quot;&quot;))&quot;;
                     obj.Worksheets[0].Cells[&quot;Z&quot; + (rowCount + startIdx)].Formula = FormulaBerthCall;
                     obj.Worksheets[0].Cells[&quot;Z&quot; + (rowCount + startIdx)].SetStyle(objStyleColor);

                     FormulaTimeatBerth = &quot;=IF(OR(V&quot; + CellNo.ToString() + @&quot;=&quot;&quot;&quot;&quot;,O&quot; + CellNo.ToString() + @&quot;=&quot;&quot;&quot;&quot;),&quot;&quot;&quot;&quot;,IF(V&quot; + CellNo.ToString() + &quot;&gt;O&quot; + CellNo.ToString() + &quot;,V&quot; + CellNo.ToString() + &quot;-O&quot; + CellNo.ToString() + @&quot;,&quot;&quot;&quot;&quot;))&quot;;
                     obj.Worksheets[0].Cells[&quot;AA&quot; + (rowCount + startIdx)].Formula = FormulaTimeatBerth;
                     obj.Worksheets[0].Cells[&quot;AA&quot; + (rowCount + startIdx)].SetStyle(objStyleTime);

                     FormulaNORTendered_AllFast = &quot;=IF(OR(Q&quot; + CellNo.ToString() + @&quot;=&quot;&quot;&quot;&quot;,P&quot; + CellNo.ToString() + @&quot;=&quot;&quot;&quot;&quot;),&quot;&quot;&quot;&quot;,IF((Q&quot; + CellNo.ToString() + &quot;-P&quot; + CellNo.ToString() + &quot;)&gt;0,Q&quot; + CellNo.ToString() + &quot;-P&quot; + CellNo.ToString() + @&quot;,0))&quot;;
                     obj.Worksheets[0].Cells[&quot;AB&quot; + (rowCount + startIdx)].Formula = FormulaNORTendered_AllFast;
                     obj.Worksheets[0].Cells[&quot;AB&quot; + (rowCount + startIdx)].SetStyle(objStyleTime);

                     FormulaAllFast_HoseConnected = &quot;=IF(OR(R&quot; + CellNo.ToString() + @&quot;=&quot;&quot;&quot;&quot;,Q&quot; + CellNo.ToString() + @&quot;=&quot;&quot;&quot;&quot;),&quot;&quot;&quot;&quot;,IF((R&quot; + CellNo.ToString() + &quot;-Q&quot; + CellNo.ToString() + &quot;)&gt;0,R&quot; + CellNo.ToString() + &quot;-Q&quot; + CellNo.ToString() + @&quot;,0))&quot;;
                     obj.Worksheets[0].Cells[&quot;AC&quot; + (rowCount + startIdx)].Formula = FormulaAllFast_HoseConnected;
                     obj.Worksheets[0].Cells[&quot;AC&quot; + (rowCount + startIdx)].SetStyle(objStyleTime);

                     FormulaHoseConnected_CargoOpsCommence = &quot;=IF(OR(S&quot; + CellNo.ToString() + @&quot;=&quot;&quot;&quot;&quot;,R&quot; + CellNo.ToString() + @&quot;=&quot;&quot;&quot;&quot;),&quot;&quot;&quot;&quot;,IF((S&quot; + CellNo.ToString() + &quot;-R&quot; + CellNo.ToString() + &quot;)&gt;0,S&quot; + CellNo.ToString() + &quot;-R&quot; + CellNo.ToString() + @&quot;,0))&quot;;
                     obj.Worksheets[0].Cells[&quot;AD&quot; + (rowCount + startIdx)].Formula = FormulaHoseConnected_CargoOpsCommence;
                     obj.Worksheets[0].Cells[&quot;AD&quot; + (rowCount + startIdx)].SetStyle(objStyleTime);

                     FormulaCargoOps = &quot;=IF(OR(T&quot; + CellNo.ToString() + @&quot;=&quot;&quot;&quot;&quot;,S&quot; + CellNo.ToString() + @&quot;=&quot;&quot;&quot;&quot;),&quot;&quot;&quot;&quot;,IF((T&quot; + CellNo.ToString() + &quot;-S&quot; + CellNo.ToString() + &quot;)&gt;0,T&quot; + CellNo.ToString() + &quot;-S&quot; + CellNo.ToString() + @&quot;,0))&quot;;
                     obj.Worksheets[0].Cells[&quot;AE&quot; + (rowCount + startIdx)].Formula = FormulaCargoOps;
                     obj.Worksheets[0].Cells[&quot;AE&quot; + (rowCount + startIdx)].SetStyle(objStyleTime);

                     FormulaCargoOps_HoseDisconnect = &quot;=IF(OR(U&quot; + CellNo.ToString() + @&quot;=&quot;&quot;&quot;&quot;,T&quot; + CellNo.ToString() + @&quot;=&quot;&quot;&quot;&quot;),&quot;&quot;&quot;&quot;,IF((U&quot; + CellNo.ToString() + &quot;-T&quot; + CellNo.ToString() + &quot;)&gt;0,U&quot; + CellNo.ToString() + &quot;-T&quot; + CellNo.ToString() + @&quot;,0))&quot;;
                     obj.Worksheets[0].Cells[&quot;AF&quot; + (rowCount + startIdx)].Formula = FormulaCargoOps_HoseDisconnect;
                     obj.Worksheets[0].Cells[&quot;AF&quot; + (rowCount + startIdx)].SetStyle(objStyleTime);

                     FormulaHoseDisconnected_AllLinesOnDeck = &quot;=IF(OR(V&quot; + CellNo.ToString() + @&quot;=&quot;&quot;&quot;&quot;,U&quot; + CellNo.ToString() + @&quot;=&quot;&quot;&quot;&quot;),&quot;&quot;&quot;&quot;,IF((V&quot; + CellNo.ToString() + &quot;-U&quot; + CellNo.ToString() + &quot;)&gt;0,V&quot; + CellNo.ToString() + &quot;-U&quot; + CellNo.ToString() + @&quot;,0))&quot;;
                     obj.Worksheets[0].Cells[&quot;AG&quot; + (rowCount + startIdx)].Formula = FormulaHoseDisconnected_AllLinesOnDeck;
                     obj.Worksheets[0].Cells[&quot;AG&quot; + (rowCount + startIdx)].SetStyle(objStyleTime);

                     rowCount++;
                 }

                 // BP

                 try
                 {
                     PivotTableCollection pivotTables = obj.Worksheets[&quot;BP&quot;].PivotTables;
                     string pivotDataSourceArea = &quot;DATA!A8:&quot; + obj.Worksheets[&quot;DATA&quot;].Cells[dtDetails.Rows.Count + 7, dtDetails.Columns.Count - 1].Name;
                     string startingCell = &quot;A36&quot;;
                     string pivotTableName = &quot;PivotTable&quot;;
                     int index = pivotTables.Add(pivotDataSourceArea, startingCell, pivotTableName);
                     PivotTable pivotTable = pivotTables[index];

                     pivotTable.RowFields.AddByBaseIndex(dtDetails.Columns[&quot;Terminal/Berth - First line ashore&quot;].Ordinal);
                     pivotTable.RowFields.AddByBaseIndex(dtDetails.Columns[&quot;PortLog - Terminal/Berth/ETA&quot;].Ordinal);
                     pivotTable.RowFields.AddByBaseIndex(dtDetails.Columns[&quot;Cargo Activity&quot;].Ordinal);
                     pivotTable.RowFields.AddByBaseIndex(dtDetails.Columns[&quot;PortLog - Cargo No&quot;].Ordinal);
                     pivotTable.RowFields.AddByBaseIndex(dtDetails.Columns[&quot;PortLog - Trade Name&quot;].Ordinal);

                     pivotTable.DataFields.AddByBaseIndex(dtDetails.Columns[&quot;All Fast&quot;].Ordinal);
                     pivotTable.DataFields.AddByBaseIndex(dtDetails.Columns[&quot;All Fast to hose connected&quot;].Ordinal);
                     pivotTable.DataFields.AddByBaseIndex(dtDetails.Columns[&quot;Hose connected to cargo ops commence&quot;].Ordinal);
                     pivotTable.DataFields.AddByBaseIndex(dtDetails.Columns[&quot;Cargo Ops&quot;].Ordinal);
                     pivotTable.DataFields.AddByBaseIndex(dtDetails.Columns[&quot;Cargo Ops to hose disconnect&quot;].Ordinal);
                     pivotTable.DataFields.AddByBaseIndex(dtDetails.Columns[&quot;Hose disconnected to all lines on deck&quot;].Ordinal);


                     PivotField pivotDataField1 = pivotTable.DataFields[0];
                     pivotDataField1.Function = ConsolidationFunction.Min;
                     pivotDataField1.NumberFormat = &quot;dd-mmm-yy hh:mm&quot;;

                     PivotField pivotDataField2 = pivotTable.DataFields[1];
                     pivotDataField2.Function = ConsolidationFunction.Average;
                     pivotDataField2.NumberFormat = &quot;[hh]:mm&quot;;

                     PivotField pivotDataField3 = pivotTable.DataFields[2];
                     pivotDataField3.Function = ConsolidationFunction.Average;
                     pivotDataField3.NumberFormat = &quot;[hh]:mm&quot;;

                     PivotField pivotDataField4 = pivotTable.DataFields[3];
                     pivotDataField4.Function = ConsolidationFunction.Average;
                     pivotDataField4.NumberFormat = &quot;[hh]:mm&quot;;

                     PivotField pivotDataField5 = pivotTable.DataFields[4];
                     pivotDataField5.Function = ConsolidationFunction.Average;
                     pivotDataField5.NumberFormat = &quot;[hh]:mm&quot;;

                     PivotField pivotDataField6 = pivotTable.DataFields[5];
                     pivotDataField6.Function = ConsolidationFunction.Average;
                     pivotDataField6.NumberFormat = &quot;[hh]:mm&quot;;

                     pivotTable.AddFieldToArea(PivotFieldType.Column, pivotTable.DataField);
                     pivotTable.ShowColumnGrandTotals = false;


                     Aspose.Cells.Style DataStyle = obj.CreateStyle();

                     DataStyle.Font.Size = 8;
                     DataStyle.Font.Name = &quot;Arial&quot;;
                     DataStyle.Font.Color = Color.Black;
                     DataStyle.RotationAngle = 90;

                     pivotTable.AutoFormatType = PivotTableAutoFormatType.Classic;

                     pivotTable.DataFields[0].DisplayName = &quot;All Fast &quot;;
                     pivotTable.DataFields[1].DisplayName = &quot;All fast to hose connected&quot;;
                     pivotTable.DataFields[2].DisplayName = &quot;Hose conn - cargo ops commence&quot;;
                     pivotTable.DataFields[3].DisplayName = &quot;Cargo Ops&quot;;
                     pivotTable.DataFields[4].DisplayName = &quot;Cargo Ops complete - hose disconnect&quot;;
                     pivotTable.DataFields[5].DisplayName = &quot;Hose disconnected to all lines on deck&quot;;

                     pivotTable.PageFields.AddByBaseIndex(dtDetails.Columns[&quot;Vessel Name&quot;].Ordinal);
                     pivotTable.PageFields.AddByBaseIndex(dtDetails.Columns[&quot;Cargo details-Voyage No&quot;].Ordinal);
                     pivotTable.PageFields.AddByBaseIndex(dtDetails.Columns[&quot;Port Name&quot;].Ordinal);
                     pivotTable.PageFields.AddByBaseIndex(dtDetails.Columns[&quot;Terminal&quot;].Ordinal);
                     pivotTable.PageFields.AddByBaseIndex(dtDetails.Columns[&quot;Berth&quot;].Ordinal);


                     pivotTable.RowFields[0].IsAutoSort = true;
                     pivotTable.RowFields[1].IsAutoSort = true;
                     pivotTable.RowFields[2].IsAutoSort = true;

                     pivotTable.PageFields[0].IsAutoSort = true;
                     pivotTable.PageFields[1].IsAutoSort = true;
                     pivotTable.PageFields[2].IsAutoSort = true;
                     pivotTable.PageFields[3].IsAutoSort = true;
                     pivotTable.PageFields[4].IsAutoSort = true;

                     obj.Worksheets[&quot;BP&quot;].PivotTables[0].RowFields[0].IsAutoSubtotals = false;
                     obj.Worksheets[&quot;BP&quot;].PivotTables[0].RowFields[1].IsAutoSubtotals = false;
                     obj.Worksheets[&quot;BP&quot;].PivotTables[0].RowFields[2].IsAutoSubtotals = false;
                     obj.Worksheets[&quot;BP&quot;].PivotTables[0].RowFields[3].IsAutoSubtotals = false;
                     obj.Worksheets[&quot;BP&quot;].PivotTables[0].RowFields[0].ShowInOutlineForm = false;
                     obj.Worksheets[&quot;BP&quot;].PivotTables[0].ShowRowHeaderCaption = false;
                     obj.Worksheets[&quot;BP&quot;].PivotTables[0].RowFields[0].NumberFormat = &quot;m/d/yyyy h:mm&quot;;
                     obj.Worksheets[&quot;BP&quot;].PivotTables[0].DisplayErrorString = true;
                     obj.Worksheets[&quot;BP&quot;].PivotTables[0].RowFields[0].ShowInOutlineForm = false;
                     obj.Worksheets[&quot;BP&quot;].PivotTables[0].ShowRowHeaderCaption = false;

                     obj.Worksheets[&quot;BP&quot;].Charts.Add(ChartType.BarStacked, 2, 0, 25, 10);
                     obj.Worksheets[&quot;BP&quot;].Charts[0].PivotSource = &quot;BP!PivotTable&quot;;
                     obj.Worksheets[&quot;BP&quot;].Charts[0].ChartArea.Area.ForegroundColor = Color.White;
                     obj.Worksheets[&quot;BP&quot;].Charts[0].PlotArea.Area.ForegroundColor = Color.White;
                     obj.Worksheets[&quot;BP&quot;].Charts[0].Title.Text = &quot;&quot;;
                     obj.Worksheets[&quot;BP&quot;].Charts[0].ShowLegend = true;
                     obj.Worksheets[&quot;BP&quot;].Charts[0].Legend.Position = LegendPositionType.Top;
                     obj.Worksheets[&quot;BP&quot;].Charts[0].ValueAxis.TickLabels.RotationAngle = 45;
                     obj.Worksheets[&quot;BP&quot;].Charts[0].ValueAxis.TickLabels.Font.IsBold = false;
                     obj.Worksheets[&quot;BP&quot;].Charts[0].ValueAxis.TickLabelPosition = TickLabelPositionType.NextToAxis;
                     obj.Worksheets[&quot;BP&quot;].Charts[0].ValueAxis.MajorTickMark = TickMarkType.Outside;
                     obj.Worksheets[&quot;BP&quot;].Charts[0].ValueAxis.MinorTickMark = TickMarkType.None;

                     obj.Worksheets[&quot;BP&quot;].Charts[0].CategoryAxis.IsPlotOrderReversed = true;
                     obj.Worksheets[&quot;BP&quot;].Charts[0].CategoryAxis.HasMultiLevelLabels = true;
                     obj.Worksheets[&quot;BP&quot;].Charts[0].CategoryAxis.MajorTickMark = TickMarkType.Inside;
                     obj.Worksheets[&quot;BP&quot;].Charts[0].CategoryAxis.MinorTickMark = TickMarkType.None;
                     obj.Worksheets[&quot;BP&quot;].Charts[0].CategoryAxis.TickLabelPosition = TickLabelPositionType.NextToAxis;

                 }
                 catch (Exception ex)
                 {
                     obj.Worksheets[&quot;BP&quot;].RemoveAllDrawingObjects();
                     obj.Worksheets[&quot;BP&quot;].Cells.ClearContents(0, 0, 2000, 2000);
                     obj.Worksheets[&quot;BP&quot;].Cells[0, 0].Value = &quot;No data to create pivot table and pivot chart&quot;;// &quot;Exception Occurred&quot;;
                 }


             }
             //obj.Save(&quot;Output.xlsx&quot;, SaveType.OpenInBrowser, FileFormatType.Xlsx, HttpContext.Current.Response);
             obj.Save(outfn, SaveFormat.Xlsx);
#if WTEST
            Process.Start(&quot;explorer.exe&quot;, string.Format(&quot;\&quot;{0}\&quot;&quot;, outfn));
#endif
         }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


