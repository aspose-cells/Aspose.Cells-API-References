---
title: WriteProtection.ValidatePassword
second_title: Aspose.Cells for .NET API Reference
description: WriteProtection method. Returns true if the specified password is the same as the writeprotection password the file was protected with
type: docs
url: /net/aspose.cells/writeprotection/validatepassword/
---
## WriteProtection.ValidatePassword method

Returns true if the specified password is the same as the write-protection password the file was protected with.

```csharp
public bool ValidatePassword(string password)
```

| Parameter | Type | Description |
| --- | --- | --- |
| password | String | The specified password. |

### Examples

```csharp
// Called: Assert.IsTrue(workbook.Settings.WriteProtection.ValidatePassword(&amp;quot;5678&amp;quot;));
[Test]
        public void Method_String_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet43261.xlsb&quot;);
            Assert.IsTrue(workbook.Settings.WriteProtection.IsWriteProtected);
            Assert.IsTrue(workbook.Settings.WriteProtection.ValidatePassword(&quot;5678&quot;));
            workbook.Save(Constants.destPath + &quot;CellsNet43261.xlsb&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CellsNet43261.xlsb&quot;);
            Assert.IsTrue(workbook.Settings.WriteProtection.IsWriteProtected);
            Assert.IsTrue(workbook.Settings.WriteProtection.ValidatePassword(&quot;5678&quot;)); 
        }
```

### See Also

* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


