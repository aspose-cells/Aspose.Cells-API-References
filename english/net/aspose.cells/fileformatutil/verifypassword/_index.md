---
title: FileFormatUtil.VerifyPassword
second_title: Aspose.Cells for .NET API Reference
description: FileFormatUtil method. Detects and returns the information about a format of an excel stored in a stream
type: docs
url: /net/aspose.cells/fileformatutil/verifypassword/
---
## FileFormatUtil.VerifyPassword method

Detects and returns the information about a format of an excel stored in a stream.

```csharp
public static bool VerifyPassword(Stream stream, string password)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream |  |
| password | String | The password for encrypted ooxml files. |

### Return Value

Returns whether the password is corrected.

### Examples

```csharp
// Called: Assert.IsTrue(FileFormatUtil.VerifyPassword(stream, "test"));
public void FileFormatUtil_Method_VerifyPassword()
{
    using (Stream stream = File.OpenRead(Constants.sourcePath + "example.xlsx"))
    {
     //  FileFormatInfo info = FileFormatUtil.DetectFileFormat(stream, "test");
        Assert.IsTrue(FileFormatUtil.VerifyPassword(stream, "test"));
      //  Assert.IsTrue(info.IsPasswordValid);
    }
    using (Stream stream = File.OpenRead(Constants.sourcePath + "example.xlsx"))
    {
        FileFormatInfo info = FileFormatUtil.DetectFileFormat(stream, "1234");
        Assert.IsTrue(info.IsEncrypted);
       // Assert.IsFalse(info.IsPasswordValid);
    }
}
```

### See Also

* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


