---
title: ListBoxActiveXControl.ListStyle
second_title: Aspose.Cells for .NET API Reference
description: ListBoxActiveXControl property. Gets and sets the visual appearance
type: docs
url: /net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/liststyle/
---
## ListBoxActiveXControl.ListStyle property

Gets and sets the visual appearance.

```csharp
public ControlListStyle ListStyle { get; set; }
```

### Examples

```csharp
// Called: list.ListStyle = (ControlListStyle.Option);
public void ListBoxActiveXControl_Property_ListStyle()
{
    Workbook workbook = new Workbook();

    String columnNumber = "5";

    //Get the first worksheet. 
    Worksheet sheet = workbook.Worksheets[0];

    //Get the worksheet cells collection. 
    Cells cells = sheet.Cells;

    //Input a value. 
    cells["B3"].Value = ("Choose Dept:");



    //Input some values that denote the input range for the combo box. 
    //cells.get("A2").setValue("Sales");
    //cells.get("A3").setValue("Finance");
    //cells.get("A4").setValue("MIS");
    //cells.get("A5").setValue("R&D");
    //cells.get("A6").setValue("Marketing");
    //cells.get("A7").setValue("HRA");

    //Access combo box, change its fill range and value property 
    Shape shape = sheet.Shapes.AddActiveXControl(ControlType.ListBox, 5, 0, 5, 0, 100, 200);
    shape.Name = ("MyList" + columnNumber);
    ListBoxActiveXControl list = (ListBoxActiveXControl)shape.ActiveXControl;

    list.ListFillRange = ("A3:A7");
    list.Value = ("Apple");
    list.LinkedCell = ("A1");
    list.ListStyle = (ControlListStyle.Option);
    list.SelectionType = (SelectionType.Multi);

    //Save the output Excel file 
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    Assert.AreEqual(workbook.Worksheets[0].Shapes[0].Name, "MyList" + columnNumber);
}
```

### See Also

* enum [ControlListStyle](../../controlliststyle/)
* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


