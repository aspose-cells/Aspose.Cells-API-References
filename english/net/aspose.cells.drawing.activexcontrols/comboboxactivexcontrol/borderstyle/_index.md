---
title: ComboBoxActiveXControl.BorderStyle
second_title: Aspose.Cells for .NET API Reference
description: ComboBoxActiveXControl property. Gets and set the type of border used by the control
type: docs
url: /net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/borderstyle/
---
## ComboBoxActiveXControl.BorderStyle property

Gets and set the type of border used by the control.

```csharp
public ControlBorderType BorderStyle { get; set; }
```

### Examples

```csharp
// Called: c.BorderStyle = Aspose.Cells.Drawing.ActiveXControls.ControlBorderType.None;
[Test]
        public void Property_BorderStyle()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Style style;
            StyleFlag flag;

            for (int i = 0; i <= 255; i++)
            {
                style = sheet.Cells.Columns[(byte)i].GetStyle();
                style.IsLocked = false;
                flag = new StyleFlag();
                flag.Locked = true;
                sheet.Cells.Columns[(byte)i].ApplyStyle(style, flag);
            }

            style = sheet.Cells.Columns[0].GetStyle();
            style.IsLocked = true;
            flag = new StyleFlag();
            flag.Locked = true;
            sheet.Cells.Columns[0].ApplyStyle(style, flag);

            Aspose.Cells.Drawing.Shape s = sheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 5, 0, 5, 0, 100, 20);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl c = (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)s.ActiveXControl;
            s.ActiveXControl.IsLocked = false;
            c.IsVisible = true;
            c.BorderStyle = Aspose.Cells.Drawing.ActiveXControls.ControlBorderType.None;
            c.Font.Name = "Arial";
            c.Font.Color = System.Drawing.Color.Black;
            c.ListRows = 12;
            c.MatchEntry = Aspose.Cells.Drawing.ActiveXControls.ControlMatchEntryType.None;

            sheet.Protect(ProtectionType.All);
            wb.Save(Constants.destPath + "CellsNet45183.xlsb", SaveFormat.Xlsb);
            wb = new Workbook(Constants.destPath + "CellsNet45183.xlsb");

            sheet = wb.Worksheets[0];
            Aspose.Cells.Drawing.Shape s0 = sheet.Shapes[0];
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl c0 = (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)s0.ActiveXControl;
            Assert.AreEqual(s0.ActiveXControl.IsLocked,false);
        }
```

### See Also

* enum [ControlBorderType](../../controlbordertype/)
* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


