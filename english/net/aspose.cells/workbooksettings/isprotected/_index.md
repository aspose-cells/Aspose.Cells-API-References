---
title: WorkbookSettings.IsProtected
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Gets a value that indicates whether the structure or window of the Workbook is protected
type: docs
url: /net/aspose.cells/workbooksettings/isprotected/
---
## WorkbookSettings.IsProtected property

Gets a value that indicates whether the structure or window of the Workbook is protected.

```csharp
public bool IsProtected { get; }
```

### Examples

```csharp
// Called: Console.WriteLine(book.Settings.IsProtected);
public void WorkbookSettings_Property_IsProtected()
{
    Console.WriteLine("Test_Encrypt_94610()");
    string infn1 = path + "example.xls";
    string infn2 = path + "example.xlsm";
    string outfn1 = Constants.destPath + "example.xlsm";
    string outfn2 = Constants.destPath + "example.xlsm";
    Workbook book = new Workbook(infn1);
    Console.WriteLine(book.Settings.IsProtected);
    book.Save(outfn1);
            
    book = new Workbook(infn2);
    Console.WriteLine(book.Settings.IsProtected);
    book.Save(outfn2);

    book = new Workbook(outfn1);
    Console.WriteLine(book.Settings.IsProtected);

    book = new Workbook(outfn2);
    Console.WriteLine(book.Settings.IsProtected);
}
```

### See Also

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


