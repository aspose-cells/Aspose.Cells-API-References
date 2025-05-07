---
title: Cell.GetValidation
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Gets the validation applied to this cell
type: docs
url: /net/aspose.cells/cell/getvalidation/
---
## Cell.GetValidation method

Gets the validation applied to this cell.

```csharp
public Validation GetValidation()
```

### Examples

```csharp
// Called: Assert.AreEqual(sheetTgt2.Cells["A58"].GetValidation().Formula1,"=OR(COUNTIF(A58,\"P?.?\")>0,COUNTIF(A58,\"P?.?K\")>0,COUNTIF(A58,\"P11H\")>0)");
[Test]
        public void Method_GetValidation()
        {
            string srcFilePath = Constants.sourcePath + "CellsNet45760.xlsm";


            Workbook wb = new Workbook(srcFilePath);
            Worksheet sheetSrc = wb.Worksheets["Data"];
            Worksheet sheetTgt1 = sheetSrc;
            Worksheet sheetTgt2 = wb.Worksheets["Data2"];

            Aspose.Cells.Range sourceRange = sheetSrc.Cells.CreateRange(0, 1, true);
            Aspose.Cells.Range destRange1 = sheetTgt1.Cells.CreateRange(1, 1, true);
            Aspose.Cells.Range destRange2 = sheetTgt2.Cells.CreateRange(0, 1, true);
            PasteOptions options = new PasteOptions
            {
                PasteType = PasteType.All
            };
            // destRange1.Copy(sourceRange, options); //<-- Works 
            destRange2.Copy(sourceRange, options); //<-- Does not work correctly 
            Assert.AreEqual(sheetTgt2.Cells["A58"].GetValidation().Formula1,"=OR(COUNTIF(A58,\"P?.?\")>0,COUNTIF(A58,\"P?.?K\")>0,COUNTIF(A58,\"P11H\")>0)");
            wb.Save(Constants.destPath + "CellsNet45760.xlsm"); 
        }
```

### See Also

* class [Validation](../../validation/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


