---
title: SeriesCollection.IsColorVaried
second_title: Aspose.Cells for .NET API Reference
description: SeriesCollection property. Represents if the color of points is varied
type: docs
url: /net/aspose.cells.charts/seriescollection/iscolorvaried/
---
## SeriesCollection.IsColorVaried property

Represents if the color of points is varied.

```csharp
public bool IsColorVaried { get; set; }
```

### Examples

```csharp
// Called: chart.NSeries.IsColorVaried = true;
[Test]
        public void Property_IsColorVaried()
        {
            Workbook workbook = new Workbook();  
            //Set default font                 
            Style style = workbook.DefaultStyle;   
            style.Font.Name = &quot;Tahoma&quot;;                 
            workbook.DefaultStyle = style;             
            Worksheet sheet = workbook.Worksheets[0];      
            //Set the name of worksheet                 
            sheet.Name = &quot;Data&quot;;               
            Cells cells = workbook.Worksheets[0].Cells;    
            //Put a value into a cell                 
            cells[&quot;A1&quot;].PutValue(&quot;Region&quot;);              
            cells[&quot;A2&quot;].PutValue(&quot;France&quot;);               
            cells[&quot;A3&quot;].PutValue(&quot;Germany&quot;);             
            cells[&quot;A4&quot;].PutValue(&quot;England&quot;);               
            cells[&quot;A5&quot;].PutValue(&quot;USA&quot;);                  
            cells[&quot;A6&quot;].PutValue(&quot;China&quot;);         
            cells[&quot;B1&quot;].PutValue(&quot;Sale1&quot;);         
            cells[&quot;B2&quot;].PutValue(70000);             
            cells[&quot;B3&quot;].PutValue(55000);              
            cells[&quot;B4&quot;].PutValue(30000);              
            cells[&quot;B5&quot;].PutValue(85000);              
            cells[&quot;B6&quot;].PutValue(90000);              
            cells[&quot;C1&quot;].PutValue(&quot;Sale2&quot;);            
            cells[&quot;C2&quot;].PutValue(60000);              
            cells[&quot;C3&quot;].PutValue(45000);               
            cells[&quot;C4&quot;].PutValue(20000);               
            cells[&quot;C5&quot;].PutValue(65000);               
            cells[&quot;C6&quot;].PutValue(80000);               
            int sheetIndex = workbook.Worksheets.Add(); 
            sheet = workbook.Worksheets[sheetIndex];    
            //Set the name of worksheet                 
            sheet.Name = &quot;Chart&quot;;                  
            //Create chart                
            int chartIndex = 0;            
            chartIndex = sheet.Charts.Add(ChartType.Column, 1, 1, 25, 12); 
            Chart chart = sheet.Charts[chartIndex];             
            //Set properties of chart title        
            chart.Title.Text = &quot;Sales By Region&quot;; 
            chart.Title.TextFont.Color = Color.Blue;
            chart.Title.TextFont.IsBold = true;       
            chart.Title.TextFont.Size = 12;            
            //Set properties of first nseries          
            chart.NSeries.Add(&quot;Data!B2:B6&quot;, true);     
            chart.NSeries[0].Name = &quot;Sale1&quot;;           
            //Set the fill format.                 
            chart.NSeries[0].Area.FillFormat.Pattern = FillPattern.LightDownwardDiagonal; 
            chart.NSeries[0].Area.ForegroundColor = Color.Blue;            
            chart.NSeries[0].Area.BackgroundColor = Color.Yellow;       
            //Set properties of the second nseries.                 
            chart.NSeries.Add(&quot;Data!C2:C6&quot;, true);                
            chart.NSeries[1].Name = &quot;Sale2&quot;;                 
            chart.NSeries.CategoryData = &quot;Data!A2:A6&quot;;        
            chart.NSeries.IsColorVaried = true;                
            chart.PlotArea.Area.ForegroundColor = Color.White;
#if !NETCOREAPP2_0
            Bitmap bitmap = chart.ToImage();
            bitmap.Save(Constants.destPath + &quot;Test_171035.jpg&quot;, ImageFormat.Jpeg);
#endif
        }
```

### See Also

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


