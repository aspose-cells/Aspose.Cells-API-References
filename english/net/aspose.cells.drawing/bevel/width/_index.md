---
title: Bevel.Width
second_title: Aspose.Cells for .NET API Reference
description: Bevel property. Gets and sets the width of the bevel or how far into the shape it is applied. In unit of Points
type: docs
url: /net/aspose.cells.drawing/bevel/width/
---
## Bevel.Width property

Gets and sets the width of the bevel, or how far into the shape it is applied. In unit of Points.

```csharp
public double Width { get; set; }
```

### Examples

```csharp
// Called: bevel.Width = (9);
public void Bevel_Property_Width()
{
    Workbook book = new Workbook();

    //Add a Data Worksheet 
    Worksheet dataSheet = book.Worksheets.Add("DataSheet");

    //Add Chart Worksheet 
    Worksheet sheet = book.Worksheets.Add("MyChart");

    //Put some values into the cells in the data worksheet 
    dataSheet.Cells["B1"].PutValue(1);
    dataSheet.Cells["B2"].PutValue(2);
    dataSheet.Cells["B3"].PutValue(3);
    dataSheet.Cells["A1"].PutValue("A");
    dataSheet.Cells["A2"].PutValue("B");
    dataSheet.Cells["A3"].PutValue("C");

    //Define the Chart Collection 
    ChartCollection charts = sheet.Charts;

    //Add a Column chart to the Chart Worksheet 
    int chartSheetIdx = charts.Add(ChartType.Column, 5, 0, 25, 15);

    //Get the newly added Chart 
    Chart chart = book.Worksheets[2].Charts[0];


    //Hide the Legend 
    chart.ShowLegend = (false);

    //Add Data Series for the Chart 
    chart.NSeries.Add("DataSheet!B1:B3", true);
    //Specify the Category Data 
    chart.NSeries.CategoryData = ("DataSheet!A1:A3");

    //Get the Data Series 
    Series ser = chart.NSeries[0];

    //Apply the 3D formatting 
    ShapePropertyCollection spPr = ser.ShapeProperties;
    Format3D fmt3d = spPr.Format3D;

    //Specify Bevel with its height/width 
    Bevel bevel = fmt3d.TopBevel;
    bevel.Type = (BevelPresetType.Circle);
    bevel.Height = (5);
    bevel.Width = (9);

    ////Specify Surface material type 
    fmt3d.SurfaceMaterialType = (PresetMaterialType.WarmMatte);

    ////Specify surface lighting type 
    fmt3d.SurfaceLightingType = (LightRigType.ThreePoint);

    ////Specify lighting angle 
    fmt3d.LightingAngle = (20);

    //Specify Series background/foreground and line color 
    //ser.getArea().setBackgroundColor(com.aspose.cells.Color.getMaroon());
    //ser.getArea().setForegroundColor(com.aspose.cells.Color.getMaroon());
    ser.Border.Color = Color.Maroon;

    //Save the Excel file 
    Util.SaveManCheck(book, "Shape", "example.xlsx");
}
```

### See Also

* class [Bevel](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


