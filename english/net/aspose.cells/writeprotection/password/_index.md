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
// Called: workbook.Settings.WriteProtection.Password = &amp;quot;test&amp;quot;;
[Test]
        public void Property_Password()
        {
            Workbook workbook = new Workbook();
            Assert.IsFalse(workbook.Settings.WriteProtection.IsWriteProtected);
            workbook.Settings.WriteProtection.Password = &quot;test&quot;;
            Assert.IsTrue(workbook.Settings.WriteProtection.IsWriteProtected);
            workbook.Save(Constants.destPath + &quot;WriteProtect01.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;WriteProtect01.xlsx&quot;);
            Assert.IsTrue(workbook.Settings.WriteProtection.IsWriteProtected);
            workbook.Save(Constants.destPath + &quot;WriteProtect01.xls&quot;);
            workbook = new Workbook(Constants.destPath + &quot;WriteProtect01.xls&quot;);
            Assert.IsTrue(workbook.Settings.WriteProtection.IsWriteProtected);
            workbook.Save(Constants.destPath + &quot;WriteProtect01.xlsb&quot;);
            workbook = new Workbook(Constants.destPath + &quot;WriteProtect01.xlsb&quot;);
            Assert.IsTrue(workbook.Settings.WriteProtection.IsWriteProtected);
        }
```

### See Also

* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


