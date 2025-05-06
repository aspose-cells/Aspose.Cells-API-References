---
title: Validation.IgnoreBlank
second_title: Aspose.Cells for .NET API Reference
description: Validation property. Indicates whether blank values are permitted by the range data validation
type: docs
url: /net/aspose.cells/validation/ignoreblank/
---
## Validation.IgnoreBlank property

Indicates whether blank values are permitted by the range data validation.

```csharp
public bool IgnoreBlank { get; set; }
```

### Examples

```csharp
// Called: validation.IgnoreBlank = true;
[Test]
        //http://www.aspose.com/community/forums/thread/258342.aspx
        public void Property_IgnoreBlank()
        {
            Console.WriteLine(&quot;Property_IgnoreBlank()&quot;);
            string outfn = Constants.destPath + @&quot;CELLSNET-19975_out.xlsx&quot;;
            string outfn03 = Constants.destPath + @&quot;CELLSNET-19975_out.xls&quot;;

            // Create a workbook.
            Workbook workbook = new Workbook();
            Worksheet ws = workbook.Worksheets[&quot;Sheet1&quot;];


            StyleFlag flag = new StyleFlag();
            flag.NumberFormat = true;
            Style style = workbook.CreateStyle();
            style.Custom = &quot;dd/mm/yyyy&quot;;
            ws.Cells.ApplyColumnStyle(0, style, flag);

            // Obtain the cells of the first worksheet.
            Cells cells = workbook.Worksheets[0].Cells;

            // Get the validations collection.
            ValidationCollection validations = workbook.Worksheets[0].Validations;
            // Set a collection of CellArea which contains the data validation settings.
            CellArea cellArea = new CellArea();
            cellArea.StartRow = 0;
            cellArea.EndRow = 1;
            cellArea.StartColumn = 0;
            cellArea.EndColumn = 0;

          
            // Add a new validation.
            Validation validation = validations[validations.Add(cellArea)];

            // Set the data validation type.
            validation.Type = ValidationType.Date;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = &quot;11/05/2010&quot;;
            validation.Formula2 = &quot;12/05/2010&quot;;

            // Enable the error.
            validation.ShowError = true;
            validation.AlertStyle = ValidationAlertType.Stop;
            validation.ErrorTitle = &quot;Date Error&quot;;
            validation.ErrorMessage = &quot;Enter a Valid Date&quot;;
            validation.InputMessage = &quot;Date Validation Type&quot;;
            validation.IgnoreBlank = true;
            validation.ShowInput = true;

          

            // Save the excel file.
            workbook.Save(outfn, SaveFormat.Xlsx);
            workbook.Save(outfn03, SaveFormat.Excel97To2003);
            workbook = new Workbook(outfn);
            Validation vldt = workbook.Worksheets[0].Validations[0];
            Assert.AreEqual(ValidationType.Date, vldt.Type, &quot;Resaved ValidationType&quot;);
            Assert.AreEqual(&quot;2010-11-5&quot;, vldt.Formula1, &quot;Resaved ValidationFormula1&quot;);
            Assert.AreEqual(&quot;2010-12-5&quot;, vldt.Formula2, &quot;Resaved ValidationFormula2&quot;);
        }
```

### See Also

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


