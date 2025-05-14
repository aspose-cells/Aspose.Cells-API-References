---
title: Worksheet.Name
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets or sets the name of the worksheet
type: docs
url: /net/aspose.cells/worksheet/name/
---
## Worksheet.Name property

Gets or sets the name of the worksheet.

```csharp
public string Name { get; set; }
```

### Remarks

The max length of sheet name is 31. And you cannot assign same name(case insensitive) to two worksheets. For example, you cannot set "SheetName1" to the first worksheet and set "SHEETNAME1" to the second worksheet.

### Examples

```csharp
// Called: Masterbook.Worksheets.Add(ws.Name);
public void Worksheet_Property_Name()
{
    string filePath = Constants.openPivottablePath + "source(1).xlsx";

    Workbook workbook = new Workbook(filePath);
    WorksheetCollection wrksheets = workbook.Worksheets;
    //copy the workseets of the First work book to another workbook
    Workbook Masterbook = new Workbook();
    foreach (Worksheet ws in wrksheets)
    {
        Masterbook.Worksheets.Add(ws.Name);
        Masterbook.Worksheets[ws.Name].Copy(ws);
    }
    // saving the second work book to see how it is looking here RowHeaderCaption and ColumnHeaderCaption went back to the default.
    Masterbook.Save(Constants.savePivottablePath + "example.xlsx", SaveFormat.Xlsx);
}
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


