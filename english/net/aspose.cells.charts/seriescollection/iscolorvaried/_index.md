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
        public void SeriesCollection_Property_IsColorVaried()
        {
            Workbook workbook = new Workbook();  
            //Set default font                 
            Style style = workbook.DefaultStyle;   
            style.Font.Name = "Tahoma";                 
            workbook.DefaultStyle = style;             
            Worksheet sheet = workbook.Worksheets[0];      
            //Set the name of worksheet                 
            sheet.Name = "Data";               
            Cells cells = workbook.Worksheets[0].Cells;    
            //Put a value into a cell                 
            cells["A1"].PutValue("Region");              
            cells["A2"].PutValue("France");               
            cells["A3"].PutValue("Germany");             
            cells["A4"].PutValue("England");               
            cells["A5"].PutValue("USA");                  
            cells["A6"].PutValue("China");         
            cells["B1"].PutValue("Sale1");         
            cells["B2"].PutValue(70000);             
            cells["B3"].PutValue(55000);              
            cells["B4"].PutValue(30000);              
            cells["B5"].PutValue(85000);              
            cells["B6"].PutValue(90000);              
            cells["C1"].PutValue("Sale2");            
            cells["C2"].PutValue(60000);              
            cells["C3"].PutValue(45000);               
            cells["C4"].PutValue(20000);               
            cells["C5"].PutValue(65000);               
            cells["C6"].PutValue(80000);               
            int sheetIndex = workbook.Worksheets.Add(); 
            sheet = workbook.Worksheets[sheetIndex];    
            //Set the name of worksheet                 
            sheet.Name = "Chart";                  
            //Create chart                
            int chartIndex = 0;            
            chartIndex = sheet.Charts.Add(ChartType.Column, 1, 1, 25, 12); 
            Chart chart = sheet.Charts[chartIndex];             
            //Set properties of chart title        
            chart.Title.Text = "Sales By Region"; 
            chart.Title.TextFont.Color = Color.Blue;
            chart.Title.TextFont.IsBold = true;       
            chart.Title.TextFont.Size = 12;            
            //Set properties of first nseries          
            chart.NSeries.Add("Data!B2:B6", true);     
            chart.NSeries[0].Name = "Sale1";           
            //Set the fill format.                 
            chart.NSeries[0].Area.FillFormat.Pattern = FillPattern.LightDownwardDiagonal; 
            chart.NSeries[0].Area.ForegroundColor = Color.Blue;            
            chart.NSeries[0].Area.BackgroundColor = Color.Yellow;       
            //Set properties of the second nseries.                 
            chart.NSeries.Add("Data!C2:C6", true);                
            chart.NSeries[1].Name = "Sale2";                 
            chart.NSeries.CategoryData = "Data!A2:A6";        
            chart.NSeries.IsColorVaried = true;                
            chart.PlotArea.Area.ForegroundColor = Color.White;
#if !NETCOREAPP2_0
            Bitmap bitmap = chart.ToImage();
            bitmap.Save(Constants.destPath + "example.jpg", ImageFormat.Jpeg);
#endif
        }
```

### See Also

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


