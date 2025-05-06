---
title: VbaModule.Codes
second_title: Aspose.Cells for .NET API Reference
description: VbaModule property. Gets and sets the codes of module
type: docs
url: /net/aspose.cells.vba/vbamodule/codes/
---
## VbaModule.Codes property

Gets and sets the codes of module.

```csharp
public string Codes { get; set; }
```

### Examples

```csharp
// Called: module.Codes =
[Test]
        public void Property_Codes()
        {
            Workbook workbook = new Workbook();

            Worksheet sheet = workbook.Worksheets[0];



            int moduleIdx = workbook.VbaProject.Modules.Add(sheet);

            VbaModule module = workbook.VbaProject.Modules[moduleIdx];

            module.Codes =

                &quot;Sub ShowMessage()&quot; + &quot;\r\n&quot; +

                &quot;    MsgBox \&quot;Welcome to Aspose!\&quot;&quot; + &quot;\r\n&quot; +

                &quot;End Sub&quot;;



            Aspose.Cells.Drawing.Button button = sheet.Shapes.AddButton(2, 0, 2, 0, 28, 80);

            button.Placement = PlacementType.FreeFloating;

            button.Font.Name = &quot;Tahoma&quot;;

            button.Font.IsBold = true;

            button.Font.Color = Color.Blue;

            button.Text = &quot;Aspose&quot;;


            button.MacroName = &quot;Sheet1.ShowMessage&quot;;
            workbook.Save(Constants.destPath + &quot;N43880J40390.xlsm&quot;);
            workbook = new Workbook(Constants.destPath + &quot;N43880J40390.xlsm&quot;);
            Assert.AreEqual(&quot;Sheet1.ShowMessage&quot;, workbook.Worksheets[0].Shapes[0].MacroName);
        }
```

### See Also

* class [VbaModule](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


