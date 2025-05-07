---
title: WriteProtection.Password
second_title: Aspose.Cells for .NET API Reference
description: WriteProtection property. Sets the protected password to modify the file
type: docs
url: /net/aspose.cells/writeprotection/password/
---
## WriteProtection.Password property

Sets the protected password to modify the file.

```csharp
public string Password { get; set; }
```

### Examples

```csharp
// Called: workbook.Settings.WriteProtection.Password = "owner";
[Test]
        //http://www.aspose.com/community/forums/thread/310229/xlsx-write-protect-issue.aspx
        public void Property_Password()
        {
            Console.WriteLine("Property_Password()");
            string infn = path + @"CELLSNET-28363\protection.xlsx";
            string outfn = destpath + @"protection_out.xlsx";
            Workbook workbook = new Workbook(infn);
         //   workbook.Settings.WriteProtection.IsWriteProtected = true;
            workbook.Settings.WriteProtection.Password = "owner";
            workbook.Save(outfn);
        }
```

### See Also

* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


