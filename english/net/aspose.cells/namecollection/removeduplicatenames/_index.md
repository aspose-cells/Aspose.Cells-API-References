---
title: NameCollection.RemoveDuplicateNames
second_title: Aspose.Cells for .NET API Reference
description: NameCollection method. Remove the duplicate defined names
type: docs
url: /net/aspose.cells/namecollection/removeduplicatenames/
---
## NameCollection.RemoveDuplicateNames method

Remove the duplicate defined names

```csharp
public void RemoveDuplicateNames()
```

### Examples

```csharp
// Called: workbook.Worksheets.Names.RemoveDuplicateNames();
[Test]
        public void Method_RemoveDuplicateNames()
        {
            Workbook workbook = new Workbook();
            workbook = new Workbook(Constants.sourcePath + &quot;EnumType\\readBorderType.xls&quot;);

            checkBorderType_BottomBorder(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
            checkBorderType_BottomBorder(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
            checkBorderType_BottomBorder(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.SpreadsheetML);
            checkBorderType_BottomBorder(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
            workbook.Worksheets.Names.RemoveDuplicateNames();
        }
```

### See Also

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


