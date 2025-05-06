---
title: GroupBox.Shadow
second_title: Aspose.Cells for .NET API Reference
description: GroupBox property. Indicates whether the groupbox has shadow
type: docs
url: /net/aspose.cells.drawing/groupbox/shadow/
---
## GroupBox.Shadow property

Indicates whether the groupbox has shadow.

```csharp
public bool Shadow { get; set; }
```

### Examples

```csharp
// Called: box.Shadow = false;
[Test]
        public void Property_Shadow()
        {
            Workbook excelbook = new Aspose.Cells.Workbook();

            //For TEN_COUNTER = 3 To 1 Step -1

            for (int TEN_COUNTER = 1; TEN_COUNTER &lt;= 3; TEN_COUNTER++)
            {

                Aspose.Cells.Drawing.GroupBox box = excelbook.Worksheets[0].Shapes.AddGroupBox((TEN_COUNTER - 1) * 20 + 1, 0, 1, 0, 200, 250);
                //Console.WriteLine(box.LowerRightRow);
                box.Shadow = false;

                Aspose.Cells.Drawing.RadioButton radio1 = excelbook.Worksheets[0].Shapes.AddRadioButton((TEN_COUNTER - 1) * 20 + 3, 0, 2, 0, 30, 110);

                radio1.Text = TEN_COUNTER + &quot;1&quot;;

                radio1.LinkedCell = &quot;A&quot; + ((TEN_COUNTER - 1) * 20 + 1);

                Aspose.Cells.Drawing.RadioButton radio2 = excelbook.Worksheets[0].Shapes.AddRadioButton((TEN_COUNTER - 1) * 20 + 6, 0, 2, 0, 30, 110);

                radio2.Text = TEN_COUNTER + &quot;2&quot;;

                radio2.LinkedCell = &quot;A&quot; + ((TEN_COUNTER - 1) * 20 + 1);

                Aspose.Cells.Drawing.RadioButton radio3 = excelbook.Worksheets[0].Shapes.AddRadioButton((TEN_COUNTER - 1) * 20 + 9, 0, 2, 0, 30, 110);

                radio3.Text = TEN_COUNTER + &quot;3&quot;;

                radio3.LinkedCell = &quot;A&quot; + ((TEN_COUNTER - 1) * 20 + 1);

                Aspose.Cells.Drawing.Shape[] shapeobjects = new Aspose.Cells.Drawing.Shape[] { box, radio1, radio2, radio3 };

                Aspose.Cells.Drawing.GroupShape group = excelbook.Worksheets[0].Shapes.Group(shapeobjects);

            }


            excelbook.Worksheets.AddCopy(0);

            //excelbook.Worksheets(1).Cells(0, 0).PutValue(&quot;2&quot;)

            excelbook.Worksheets[1].Cells[20, 0].PutValue(3);

            excelbook.Worksheets[1].Cells[40, 0].PutValue(1);


            excelbook.Worksheets[0].Cells[40, 0].PutValue(1);

            excelbook.Worksheets[0].Cells[20, 0].PutValue(3);

            excelbook.Worksheets[0].Cells[0, 0].PutValue(2);
            excelbook.Worksheets[1].Shapes.UpdateSelectedValue();
            excelbook.Worksheets[0].Shapes.UpdateSelectedValue();
            Assert.AreEqual(true, ((RadioButton)excelbook.Worksheets[0].Shapes[2]).IsChecked);

            excelbook.Save(Constants.destPath + &quot;dest.xlsx&quot;);
        }
```

### See Also

* class [GroupBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


