---
title: WorkbookDesigner.LineByLine
second_title: Aspose.Cells for .NET API Reference
description: WorkbookDesigner property. Indicates whether processing the smart marker line by line
type: docs
url: /net/aspose.cells/workbookdesigner/linebyline/
---
## WorkbookDesigner.LineByLine property

Indicates whether processing the smart marker line by line.

```csharp
public bool LineByLine { get; set; }
```

### Remarks

The default value is true. If False, the template file must contain a range which is named as "_CellsSmartMarkers".

### Examples

```csharp
// Called: designer.LineByLine = (false);
public void WorkbookDesigner_Property_LineByLine()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
    ABC_1_Data res = (ABC_1_Data)JsonConvert.DeserializeObject(File.ReadAllText(Constants.sourcePath + "example.json"), typeof(ABC_1_Data));

    //		
    //wb.Worksheets[0].Cells.CreateRange("A4:K19").Name = ("_CellsSmartMarkers");
    //		// Load the data from the input json file
    List<ABC_1_Data> listFormData = new List<ABC_1_Data>();
    listFormData.Add(res);
    //		
    WorkbookDesigner designer = new WorkbookDesigner();
    designer.LineByLine = (false);
    designer.Workbook = (wb);
    designer.SetDataSource("RootData", listFormData);
    // designer.SetDataSource("Directors", res.Directors);
    designer.Process(true);
    wb.Save(Constants.destPath + "example.xlsx");
    Assert.AreEqual("Reportee", wb.Worksheets[0].Cells["A34"].StringValue);

    Assert.AreEqual("Sales", wb.Worksheets[0].Cells["K37"].StringValue);
    Assert.AreEqual("111", wb.Worksheets[0].Cells["A42"].StringValue);

}
```

### See Also

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


