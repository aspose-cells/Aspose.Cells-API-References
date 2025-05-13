---
title: Worksheet.RemoveAllDrawingObjects
second_title: Aspose.Cells for .NET API Reference
description: Worksheet method. Removes all drawing objects in this worksheet
type: docs
url: /net/aspose.cells/worksheet/removealldrawingobjects/
---
## Worksheet.RemoveAllDrawingObjects method

Removes all drawing objects in this worksheet.

```csharp
public void RemoveAllDrawingObjects()
```

### Examples

```csharp
// Called: destinationBook.Worksheets[i].RemoveAllDrawingObjects();
public void Worksheet_Method_RemoveAllDrawingObjects()
{
    Workbook templateBook = new Workbook(Constants.sourcePath + "example.xls");
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
    //destinationBook.Save(Constants.destPath + "example.xlsx");
    destinationBook.Dispose();
    templateBook.Dispose();
}
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


