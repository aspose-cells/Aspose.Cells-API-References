---
title: Axis.IsVisible
second_title: Aspose.Cells for .NET API Reference
description: Axis property. Represents if the axis is visible
type: docs
url: /net/aspose.cells.charts/axis/isvisible/
---
## Axis.IsVisible property

Represents if the axis is visible.

```csharp
public bool IsVisible { get; set; }
```

### Examples

```csharp
// Called: chart.SecondValueAxis.IsVisible = false;
[Test]
        //http://gemini.aspose.com:8042/issue/ViewIssue.aspx?ID=30987&PROJID=15
        public void Property_IsVisible()
        {
            Console.WriteLine("testCELLSNET_30987()");
            string outfn = destpath + @"demochart2.xlsx";

            Workbook wb = new Workbook();
            //Add a new worksheet to populate cells with data
            int dataSheetIdx = wb.Worksheets.Add();
            Worksheet dataSheet = wb.Worksheets[dataSheetIdx];
            string sheetName = "TotalCostOfOwnershipAvgServer";
            dataSheet.Name = sheetName;

            //  TotalCostofOwnershipServer getTotalCostOfOwnershpServerData = new TotalCostofOwnershipServer();
            //            getTotalCostOfOwnershpServerData = GetTotalCostOfOwnershpServerData();
            //ROISummaryDefaultData roisummarydefaultdata = SessionManager.Instance.ROICalculation.RoiSummaryDefaultData;
            double[][] dblData = new double[4][];

            /*            dblData[0] = new double[] { getTotalCostOfOwnershpServerData.CapEx[0], getTotalCostOfOwnershpServerData.CapEx[1] };
                        dblData[1] = new double[] { getTotalCostOfOwnershpServerData.OpEx[0], getTotalCostOfOwnershpServerData.OpEx[1] };
                        dblData[2] = new double[] { getTotalCostOfOwnershpServerData.Other[0], getTotalCostOfOwnershpServerData.Other[1] };
                        dblData[3] = new double[] { getTotalCostOfOwnershpServerData.Total[0], getTotalCostOfOwnershpServerData.Total[1] };
                */
            dblData[0] = new double[] { 100, 50 };
            dblData[1] = new double[] { 200, 120 };
            dblData[2] = new double[] { 50, 100 };
            dblData[3] = new double[] { 100, 200 };

            dataSheet.Cells[0, 0].PutValue(@"X\Y");
            dataSheet.Cells[0, 1].PutValue("Physical");
            dataSheet.Cells[0, 2].PutValue("Virtualized");
            dataSheet.Cells[1, 0].PutValue("CapEx");
            dataSheet.Cells[2, 0].PutValue("OpEx");
            dataSheet.Cells[3, 0].PutValue("Other");

            for (int i = 1; i < 5; i++)
                for (int j = 1; j < 3; j++)
                {
                    try
                    {
                        dataSheet.Cells[i, j].PutValue(dblData[i - 1][j - 1]);
                    }
                    catch (Exception ex)
                    {

                        dataSheet.Cells[i, j].PutValue(dblData[i - 1][j - 1]);
                    }

                }

            //Formatting Chart Data
            Aspose.Cells.Style style = wb.CreateStyle();
            Cells cells = dataSheet.Cells;
            Aspose.Cells.Range range = cells.CreateRange(0, 0, 3, 1);
            StyleFlag flag = new StyleFlag();
            flag.All = true;
            style.Font.IsBold = true;
            range.ApplyStyle(style, flag);
            cells[0, 1].SetStyle(style);
            cells[0, 2].SetStyle(style);

            Aspose.Cells.Style style1 = wb.CreateStyle();
            style1.Font.Color = System.Drawing.Color.FromArgb(99, 37, 35);
            cells[1, 0].SetStyle(style1);
            cells[1, 1].SetStyle(style1);
            cells[1, 2].SetStyle(style1);

            Aspose.Cells.Style style2 = wb.CreateStyle();
            style2.Font.Color = System.Drawing.Color.FromArgb(149, 55, 53);
            cells[2, 0].SetStyle(style2);
            cells[2, 1].SetStyle(style2);
            cells[2, 2].SetStyle(style2);

            Aspose.Cells.Style style3 = wb.CreateStyle();
            style3.Font.Color = System.Drawing.Color.FromArgb(217, 150, 148);
            cells[3, 0].SetStyle(style3);
            cells[3, 1].SetStyle(style3);
            cells[3, 2].SetStyle(style3);

            //Add a chart sheet
            int chartSheetIdx = wb.Worksheets.Add(SheetType.Chart);

            Worksheet chartSheet = wb.Worksheets[chartSheetIdx];
            chartSheet.Name = "ChartSheet";

            //Add a chart in ChartSheet with data series from DataSheet
            int chartIdx = 0;
            chartIdx = chartSheet.Charts.Add(Aspose.Cells.Charts.ChartType.ColumnStacked, 0, 0, 3, 3);

            Chart chart = chartSheet.Charts[chartIdx];

            chart.SizeWithWindow = true;

            for (int rows = 2; rows <= 5; rows++)
                chart.NSeries.Add(sheetName + "!B" + rows.ToString() + ":C" + rows.ToString(), false);

            Aspose.Cells.Charts.Legend legend = chart.Legend;

            legend.Position = Aspose.Cells.Charts.LegendPositionType.Bottom;

            chart.PlotArea.Area.Formatting = FormattingType.None;
            chart.PlotArea.BackgroundMode = BackgroundMode.Transparent;

            legend.Width = 400;
            legend.Height = 18;
            legend.Border.Style = Aspose.Cells.Drawing.LineType.Solid;
            legend.TextFont.Size = 12;
            chart.PlotArea.Border.IsVisible = false;
            //Set a text

            // chart.ValueAxis.DisplayUnit = DisplayUnitType.Thousands;
            chart.ValueAxis.IsDisplayUnitLabelShown = false;

            chart.ValueAxis.TickLabels.NumberFormat = System.Threading.Thread.CurrentThread.CurrentCulture.NumberFormat.CurrencySymbol + "#0.0,0";
            chart.SecondValueAxis.TickLabels.NumberFormat = "% 0";
            chart.CategoryAxis.TickLabels.NumberFormat = "#0";

            chart.PlotArea.Area.BackgroundColor = System.Drawing.Color.White;
            chart.NSeries[0].Area.ForegroundColor = ColorTranslator.FromHtml("#FF4d4d4d");// Color.FromArgb(99, 37, 35);
            chart.NSeries[1].Area.ForegroundColor = ColorTranslator.FromHtml("#FF949494");//Color.FromArgb(149, 55, 53);
            chart.NSeries[2].Area.ForegroundColor = ColorTranslator.FromHtml("#FFc9c9c9");//Color.FromArgb(217, 150, 148);

            chart.NSeries[0].Points[1].Area.ForegroundColor = ColorTranslator.FromHtml("#FF003d79");//Color.FromArgb(37, 64, 97);
            chart.NSeries[1].Points[1].Area.ForegroundColor = ColorTranslator.FromHtml("#FF0095d3");//Color.FromArgb(55, 96, 146);
            chart.NSeries[2].Points[1].Area.ForegroundColor = ColorTranslator.FromHtml("#FF7fcae9");//Color.FromArgb(149, 179, 215);

            chart.NSeries.CategoryData = "='TotalCostOfOwnershipAvgServer'!$B$1:$C$1";
            chart.ValueAxis.MajorGridLines.Transparency = .60;
            //Set properties of chart title
            chart.Title.Text = "Total Cost of Ownership:  Average per Server Workload per Hour \n (excluding any desktop workloads in analysis)";
            chart.Title.TextFont.Color = System.Drawing.Color.Black;
            chart.Title.TextFont.IsBold = true;
            chart.Title.TextFont.Size = 12;
            chart.Title.TextFont.Name = "Arial";
            chart.ValueAxis.TickLabels.Font.Name = "Arial";
            chart.CategoryAxis.TickLabels.Font.Name = "Arial";
            chart.PlotArea.TextFont.Name = "Arial";

            //Set properties of valueaxis title
            Axis valueAxis = chart.ValueAxis;
            valueAxis.TickLabels.Font.Size = 10;
            valueAxis.TickLabels.Font.Name = "Arial";

            //Set properties of Axis(categoryaxis) title
            Axis categoryAxis = chart.CategoryAxis;
            categoryAxis.TickLabels.Font.Size = 10;
            categoryAxis.TickLabels.Font.Name = "Arial";
            legend.Position = LegendPositionType.Bottom;
            Aspose.Cells.Charts.Series ser1 = chart.NSeries[0];
            Aspose.Cells.Charts.Series ser2 = chart.NSeries[1];
            Aspose.Cells.Charts.Series ser3 = chart.NSeries[2];
            Aspose.Cells.Charts.Series ser4 = chart.NSeries[3];
            categoryAxis.TickLabelPosition = TickLabelPositionType.Low;
            categoryAxis.CategoryType = CategoryType.CategoryScale;
            ser4.PlotOnSecondAxis = true;
            //ser4.DataLabels.X = 10;
            //ser4.DataLabels.Y = -1000;

            ser1.GapWidth = 55;
            ser2.GapWidth = 55;
            ser3.GapWidth = 55;
            ser4.GapWidth = 55;
            ser4.LegendEntry.IsDeleted = true;

            DataLabels datalabels;
            for (int i = 0; i < chart.NSeries.Count; i++)
            {
                datalabels = chart.NSeries[i].DataLabels;
                //Set the position of DataLabels
                if (i != 3)
                    datalabels.Position = LabelPositionType.Above;
                //else
                //{
                //    ser4.DataLabels.TextHorizontalAlignment = TextAlignmentType.Top;
                //}
                datalabels.NumberFormat = System.Threading.Thread.CurrentThread.CurrentCulture.NumberFormat.CurrencySymbol + "#0.0,0";

                //Show the category name in the DataLabels
                datalabels.ShowCategoryName = false;
                //Show the value in the DataLabels
                datalabels.ShowValue = true;
                //Not show the percentage in the DataLabels
                datalabels.ShowPercentage = false;
                //Not show the legend key.
                datalabels.ShowLegendKey = false;
            }

            ser1.Name = "CapEx";
            ser2.Name = "OpEx";
            ser3.Name = "Other";
            //ser4.Area.FillFormat.SetType = FormatSetType.None;


            /*************************************************/
            /*************************************************/
            /*************************************************/
            /*************************************************/

            // When the following statement is Executed the generated presentation failed to open the Ole frame and throws out of memory error
            //If the line is commented then double clicking ole frame in PowerPoint opens the chart in excel

            ser4.DataLabels.Position = LabelPositionType.OutsideEnd;

            /*************************************************/
            /*************************************************/
            /*************************************************/








            //ser4.DataLabels.Position = LabelPositionType.Above;

            ser4.Area.Formatting = FormattingType.None;

            //ser4.DataLabels.X = 10;
            //ser4.DataLabels.Y = -1000;
            chart.SecondValueAxis.IsVisible = false;
            chart.PlotArea.Border.IsVisible = false;
            chart.PlotArea.Area.Formatting = FormattingType.None;
            chart.PlotArea.BackgroundMode = BackgroundMode.Transparent;
            chart.PlotArea.TextFont.Size = 10;
            chart.PlotArea.TextFont.Name = "Arial";
            chart.PlotArea.Border.Transparency = 1.0;

            //Set ChartSheet an active sheet
            wb.Worksheets.ActiveSheetIndex = chartSheetIdx;
            wb.Save(outfn);
#if WTEST
            Process.Start("explorer.exe", string.Format("\"{0}\"", outfn));
#endif
        }
```

### See Also

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


