---
title: ListBoxActiveXControl.SelectionType
second_title: Aspose.Cells for .NET API Reference
description: ListBoxActiveXControl property. Indicates whether the control permits multiple selections
type: docs
url: /net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/selectiontype/
---
## ListBoxActiveXControl.SelectionType property

Indicates whether the control permits multiple selections.

```csharp
public SelectionType SelectionType { get; set; }
```

### Examples

```csharp
// Called: list.SelectionType = (SelectionType.Multi);
[Test]
        public void Property_SelectionType()
        {
            Workbook workbook = new Workbook();

            String columnNumber = &quot;5&quot;;

            //Get the first worksheet. 
            Worksheet sheet = workbook.Worksheets[0];

            //Get the worksheet cells collection. 
            Cells cells = sheet.Cells;

            //Input a value. 
            cells[&quot;B3&quot;].Value = (&quot;Choose Dept:&quot;);



            //Input some values that denote the input range for the combo box. 
            //cells.get(&quot;A2&quot;).setValue(&quot;Sales&quot;);
            //cells.get(&quot;A3&quot;).setValue(&quot;Finance&quot;);
            //cells.get(&quot;A4&quot;).setValue(&quot;MIS&quot;);
            //cells.get(&quot;A5&quot;).setValue(&quot;R&amp;D&quot;);
            //cells.get(&quot;A6&quot;).setValue(&quot;Marketing&quot;);
            //cells.get(&quot;A7&quot;).setValue(&quot;HRA&quot;);

            //Access combo box, change its fill range and value property 
            Shape shape = sheet.Shapes.AddActiveXControl(ControlType.ListBox, 5, 0, 5, 0, 100, 200);
            shape.Name = (&quot;MyList&quot; + columnNumber);
            ListBoxActiveXControl list = (ListBoxActiveXControl)shape.ActiveXControl;

            list.ListFillRange = (&quot;A3:A7&quot;);
            list.Value = (&quot;Apple&quot;);
            list.LinkedCell = (&quot;A1&quot;);
            list.ListStyle = (ControlListStyle.Option);
            list.SelectionType = (SelectionType.Multi);

            //Save the output Excel file 
            workbook.Save(Constants.destPath + &quot;CELLSJAVA42368.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CELLSJAVA42368.xlsx&quot;);
            Assert.AreEqual(workbook.Worksheets[0].Shapes[0].Name, &quot;MyList&quot; + columnNumber);
        }
```

### See Also

* enum [SelectionType](../../../aspose.cells.drawing/selectiontype/)
* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


