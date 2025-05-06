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
[Test]
        public void Property_IsProtected()
        {
            Console.WriteLine(&quot;Test_Encrypt_94610()&quot;);
            string infn1 = path + &quot;Test_Encrypt_94610.xls&quot;;
            string infn2 = path + &quot;Test_Encrypt_94610.xlsm&quot;;
            string outfn1 = Constants.destPath + &quot;Test_Encrypt_94610_xls_out.xlsm&quot;;
            string outfn2 = Constants.destPath + &quot;Test_Encrypt_94610_xlsm_out.xlsm&quot;;
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


