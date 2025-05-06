---
title: Validation.InCellDropDown
second_title: Aspose.Cells for .NET API Reference
description: Validation property. Indicates whether data validation displays a dropdown list that contains acceptable values
type: docs
url: /net/aspose.cells/validation/incelldropdown/
---
## Validation.InCellDropDown property

Indicates whether data validation displays a drop-down list that contains acceptable values.

```csharp
public bool InCellDropDown { get; set; }
```

### Examples

```csharp
// Called: list.InCellDropDown = (true);
[Test]
        public void Property_InCellDropDown()
        {
            Workbook workbook = new Workbook();

            //write the options
            Cells cells = workbook.Worksheets[0].Cells;
            int row = 0;
            for (; row &lt; 3; row++)
            {
                for (int col = 0; col &lt; 2; col++)
                {
                    cells[row, col].PutValue(row + &quot;a&quot; + col);
                }
            }
            //create named ranges for the options
            cells.CreateRange(&quot;A1&quot;, &quot;A3&quot;).Name = (&quot;options1&quot;);
            cells.CreateRange(&quot;B1&quot;, &quot;B3&quot;).Name = (&quot;options2&quot;);

            ValidationCollection validations = workbook.Worksheets[0].Validations;

            CellArea area = new CellArea();//area for option list 1
            area.StartColumn = 0;
            area.StartRow = row + 1;
            area.EndColumn = 0;
            area.EndRow = row + 10;

            //create the 1st drop down validation
            Validation list = validations[validations.Add(area)];
            list.Type = (ValidationType.List);
            list.InCellDropDown = (true);
            list.IgnoreBlank = (true);
            list.Formula1 = (&quot;=options1&quot;);

            area = new CellArea();  //area for option list 2
            area.StartColumn = 1;
            area.StartRow = row + 1;
            area.EndColumn = 1;
            area.EndRow = row + 10;

            //create the 2nd drop down validation
            list = validations[validations.Add(area)];
            list.Type = (ValidationType.List);
            list.InCellDropDown = (true);
            list.IgnoreBlank = (true);
            list.Formula1 = (&quot;=options2&quot;);

            workbook.Save(Constants.destPath + &quot;Cells41488.xls&quot;);
            workbook = new Workbook(Constants.destPath + &quot;Cells41488.xls&quot;);
            Assert.AreEqual(workbook.Worksheets[0].Validations.Count, 2);
        }
```

### See Also

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


