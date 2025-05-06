---
title: PivotTable.PivotTableStyleType
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Gets and sets the builtin pivot table style
type: docs
url: /net/aspose.cells.pivot/pivottable/pivottablestyletype/
---
## PivotTable.PivotTableStyleType property

Gets and sets the built-in pivot table style.

```csharp
public PivotTableStyleType PivotTableStyleType { get; set; }
```

### Examples

```csharp
// Called: wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleDark24;
[Test]
        public void Property_PivotTableStyleType()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET42919_&quot;;
            var wb = new Workbook(filePath + &quot;Book2.xlsx&quot;);
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B6&quot;].StringValue, &quot;A&quot;);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].StringValue, &quot;D&quot;);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;E8&quot;].StringValue, &quot;(All)&quot;);
            wb.Save(Constants.PivotTableDestPath + @&quot;NET429192.xlsx&quot;);

            wb = new Workbook(filePath + &quot;Book3.xlsx&quot;);
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B5&quot;].StringValue, &quot;A&quot;);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B8&quot;].StringValue, &quot;D&quot;);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;E8&quot;].StringValue, &quot;(All)&quot;);
            wb.Save(Constants.PivotTableDestPath + @&quot;NET429193.xlsx&quot;);

            wb = new Workbook(filePath + &quot;Book4.xlsx&quot;);
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].StringValue, &quot;A&quot;);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;K7&quot;].StringValue, &quot;D&quot;);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;K8&quot;].StringValue, &quot;(All)&quot;);
            wb.Save(Constants.PivotTableDestPath + @&quot;NET429194.xlsx&quot;);

            wb = new Workbook(filePath + &quot;Book1.xlsx&quot;);
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            wb.Save(Constants.PivotTableDestPath + @&quot;NET429191.xlsx&quot;);

            #region none
            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.None;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B6&quot;].StringValue, &quot;A&quot;);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;E6&quot;].StringValue, &quot;D&quot;);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;H7&quot;].StringValue, &quot;(All)&quot;);

           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.Empty);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.Empty);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A7&quot;].GetStyle().BackgroundColor, Color.Empty);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A7&quot;].GetStyle().ForegroundColor, Color.Empty);

           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().Borders[BorderType.TopBorder].Color, Color.FromArgb(0, 171, 171, 171));
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().Borders[BorderType.RightBorder].Color, Color.FromArgb(0, 171, 171, 171));
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().Borders[BorderType.BottomBorder].Color, Color.FromArgb(0, 171, 171, 171));
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().Borders[BorderType.LeftBorder].Color, Color.FromArgb(0, 171, 171, 171));

           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B6&quot;].GetStyle().Borders[BorderType.TopBorder].Color, Color.FromArgb(0, 171, 171, 171));
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B6&quot;].GetStyle().Borders[BorderType.RightBorder].Color, Color.FromArgb(0, 171, 171, 171));
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B6&quot;].GetStyle().Borders[BorderType.BottomBorder].Color, Color.FromArgb(0, 171, 171, 171));
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B6&quot;].GetStyle().Borders[BorderType.LeftBorder].Color, Color.FromArgb(0, 171, 171, 171));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919none.xlsx&quot;, SaveFormat.Xlsx);
            #endregion

            #region dark
            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleDark1;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 127, 127, 127));
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 127, 127, 127));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_dark1.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleDark2;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 37, 64, 97));
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 37, 64, 97));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_dark2.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleDark3;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 99, 37, 35));
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 99, 37, 35));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_dark3.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleDark4;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 79, 98, 40));
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 79, 98, 40));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_dark4.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleDark5;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 64, 49, 82));
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 64, 49, 82));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_dark5.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleDark6;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 33, 89, 104));
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 33, 89, 104));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_dark6.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleDark7;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 152, 72, 7));
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 152, 72, 7));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_dark7.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleDark8;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 217, 217, 217));
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 217, 217, 217));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_dark8.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleDark9;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 220, 230, 242));
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 220, 230, 242));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_dark9.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleDark10;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 242, 220, 219));
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 242, 220, 219));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_dark10.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleDark11;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 235, 241, 222));
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 235, 241, 222));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_dark11.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleDark12;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 230, 224, 236));
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 230, 224, 236));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_dark12.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleDark13;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 219, 238, 244));
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 219, 238, 244));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_dark13.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleDark14;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 253, 234, 218));
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 253, 234, 218));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_dark14.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleDark15;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 140, 140, 140));
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 140, 140, 140));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_dark15.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleDark16;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(0, 79, 129, 189));
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(0, 79, 129, 189));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_dark16.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleDark17;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(0, 192, 80, 77));
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(0, 192, 80, 77));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_dark17.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleDark18;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(0, 155, 187, 89));
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(0, 155, 187, 89));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_dark18.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleDark19;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(0, 128, 100, 162));
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(0, 128, 100, 162));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_dark19.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleDark20;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(0, 75, 172, 198));
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(0, 75, 172, 198));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_dark20.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleDark21;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(0, 247, 150, 70));
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(0, 247, 150, 70));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_dark21.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleDark22;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 127, 127, 127));
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 128, 128, 128));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_dark22.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleDark23;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 55, 96, 146));
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(0, 79, 129, 189));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_dark23.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleDark24;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 149, 55, 53));
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(0, 192, 80, 77));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_dark24.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleDark25;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 119, 147, 60));
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(0, 155, 187, 89));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_dark25.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleDark26;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 96, 74, 123));
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(0, 128, 100, 162));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_dark26.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleDark27;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 49, 133, 156));
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(0, 75, 172, 198));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_dark27.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleDark28;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 228, 108, 10));
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(0, 247, 150, 70));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_dark28.xlsx&quot;, SaveFormat.Xlsx);
            #endregion

            #region light
            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleLight1;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.Empty);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.Empty);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.Empty);
           AssertHelper.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.Empty);
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_light1.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleLight2;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.Empty);
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_light2.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleLight3;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.Empty);
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_light3.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleLight4;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.Empty);
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_light4.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleLight5;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.Empty);
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_light5.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleLight6;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.Empty);
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_light6.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleLight7;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.Empty);
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_light7.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleLight8;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.Empty);
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_light8.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleLight9;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.Empty);
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_light9.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleLight10;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.Empty);
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_light10.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleLight11;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.Empty);
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_light11.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleLight12;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.Empty);
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_light12.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleLight13;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.Empty);
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_light13.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleLight14;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.Empty);
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_light14.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleLight15;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 217, 217, 217));
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 217, 217, 217));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_light15.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleLight16;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 220, 230, 242));
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 220, 230, 242));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_light16.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleLight17;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 242, 220, 219));
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 242, 220, 219));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_light17.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleLight18;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 235, 241, 222));
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 235, 241, 222));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_light18.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleLight19;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 230, 224, 236));
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 230, 224, 236));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_light19.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleLight20;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 219, 238, 244));
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 219, 238, 244));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_light20.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleLight21;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 253, 234, 218));
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 253, 234, 218));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_light21.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleLight22;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.Empty);
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_light22.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleLight23;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.Empty);
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_light23.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleLight24;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.Empty);
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_light24.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleLight25;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.Empty);
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_light25.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleLight26;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.Empty);
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_light26.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleLight27;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.Empty);
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_light27.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleLight28;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.Empty);
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_light28.xlsx&quot;, SaveFormat.Xlsx);
            #endregion

            #region medium
            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium1;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.Empty);
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_medium1.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium2;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.Empty);
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_medium2.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium3;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.Empty);
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_medium3.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium4;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.Empty);
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_medium4.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium5;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.Empty);
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_medium5.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium6;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.Empty);
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_medium6.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium7;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.Empty);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.Empty);
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_medium7.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium8;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 217, 217, 217));
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 217, 217, 217));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_medium8.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium9;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 220, 230, 242));
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 220, 230, 242));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_medium9.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 242, 220, 219));
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 242, 220, 219));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_medium10.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium11;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 235, 241, 222));
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 235, 241, 222));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_medium11.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium12;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 230, 224, 236));
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 230, 224, 236));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_medium12.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium13;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 219, 238, 244));
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 219, 238, 244));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_medium13.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium14;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 253, 234, 218));
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 253, 234, 218));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_medium14.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium15;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 242, 242, 242));
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 242, 242, 242));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_medium15.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium16;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 220, 230, 242));
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 220, 230, 242));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_medium16.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium17;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 242, 220, 219));
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 242, 220, 219));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_medium17.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium18;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 235, 241, 222));
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 235, 241, 222));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_medium18.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium19;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 230, 224, 236));
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 230, 224, 236));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_medium19.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium20;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 219, 238, 244));
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 219, 238, 244));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_medium20.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium21;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 253, 234, 218));
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 253, 234, 218));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_medium21.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium22;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 191, 191, 191));
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 217, 217, 217));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_medium22.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium23;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 185, 205, 229));
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 220, 230, 242));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_medium23.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium24;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 230, 185, 184));
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 242, 220, 219));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_medium24.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium25;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 215, 228, 189));
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 235, 241, 222));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_medium25.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium26;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 204, 193, 218));
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 230, 224, 236));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_medium26.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium27;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 183, 222, 232));
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 219, 238, 244));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_medium27.xlsx&quot;, SaveFormat.Xlsx);

            wb.Worksheets[0].PivotTables[0].PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium28;
            wb.Worksheets[0].PivotTables[0].RefreshData();
            wb.Worksheets[0].PivotTables[0].CalculateData();
            wb.Worksheets[0].PivotTables[0].RefreshDataOnOpeningFile = false;
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A6&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 252, 213, 181));
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().BackgroundColor, Color.White);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B7&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 253, 234, 218));
            wb.Save(Constants.PivotTableDestPath + @&quot;NET42919_medium28.xlsx&quot;, SaveFormat.Xlsx);
            #endregion
        }
```

### See Also

* enum [PivotTableStyleType](../../pivottablestyletype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


