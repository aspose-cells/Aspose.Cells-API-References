---
title: Workbook.Dispose
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Performs applicationdefined tasks associated with freeing releasing or resetting unmanaged resources
type: docs
url: /net/aspose.cells/workbook/dispose/
---
## Workbook.Dispose method

Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources.

```csharp
public void Dispose()
```

### Examples

```csharp
// Called: workbook.Dispose();
[Test]
        public void Method_Dispose()
        {
            Workbook templateBook = new Workbook(Constants.sourcePath + "CELLSJAVA43171.xls");
            Workbook destinationBook = new Workbook();
            CopyOptions copyOptions = new CopyOptions();
            for (int i = 0; i < 2; i++)
            {
                Workbook workbook = new Workbook();
                workbook.Copy(templateBook);
                Worksheet sourceSheet = workbook.Worksheets[0];
                Worksheet destinationSheet = i == 0 ? destinationBook.Worksheets[0] : destinationBook.Worksheets.Add("sheet" + (i + 1));
                destinationSheet.Copy(sourceSheet);
                PageSetup pageSetup = destinationSheet.PageSetup;
                pageSetup.Copy(sourceSheet.PageSetup, copyOptions);
                //pageSetup.PrinterSettings= (null);
                // Or I get an error "Removed Records: Object from /xl/printerSettings/printerSettings1.bin part (Print options)"
                workbook.Dispose();
            }
            for (int i = 1; i < destinationBook.Worksheets.Count; i++)
            {
                destinationBook.Worksheets[i].RemoveAllDrawingObjects();
            }
            Util.ReSave(destinationBook, SaveFormat.Xlsx);
            //destinationBook.Save(Constants.destPath + "CELLSJAVA43171.xlsx");
            destinationBook.Dispose();
            templateBook.Dispose();
        }
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


