---
title: PageSetup.PrintArea
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. Represents the range to be printed
type: docs
url: /net/aspose.cells/pagesetup/printarea/
---
## PageSetup.PrintArea property

Represents the range to be printed.

```csharp
public string PrintArea { get; set; }
```

### Examples

```csharp
// Called: Console.WriteLine(outBook.Worksheets[0].PageSetup.PrintArea);
[Test]
        public void Property_PrintArea()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet46305.xlsx");
            var formatSheet = workbook.Worksheets[0];
            var outBook = new Workbook();
            for (int i = 1; i <= 3; i++)
            {
                outBook.Worksheets.Add();
                outBook.Worksheets[i].Copy(formatSheet);
                //Data embedding outside the print range 
                outBook.Worksheets[i].Cells["A100"].Value = "OUT OF RANGE";
                Console.WriteLine(outBook.Worksheets[0].PageSetup.PrintArea);
            }
            Console.WriteLine(outBook.Worksheets[0].PageSetup.PrintArea);
            outBook.Worksheets.RemoveAt(0);
            Assert.AreEqual(outBook.Worksheets[0].PageSetup.PrintArea, "A1:K36");
           // outBook.Save(dir + "dest.xlsx", SaveFormat.Xlsx);
            outBook.Save(Constants.destPath + "dest.pdf", Aspose.Cells.SaveFormat.Pdf);
        }
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


