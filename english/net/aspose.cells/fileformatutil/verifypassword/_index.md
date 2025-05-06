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
// Called: Assert.IsTrue(FileFormatUtil.VerifyPassword(stream, &amp;quot;test&amp;quot;));
[Test]
        public void Method_String_()
        {
            using (Stream stream = File.OpenRead(Constants.sourcePath + &quot;CellsNet47625.xlsx&quot;))
            {
             //  FileFormatInfo info = FileFormatUtil.DetectFileFormat(stream, &quot;test&quot;);
                Assert.IsTrue(FileFormatUtil.VerifyPassword(stream, &quot;test&quot;));
              //  Assert.IsTrue(info.IsPasswordValid);
            }
            using (Stream stream = File.OpenRead(Constants.sourcePath + &quot;CellsNet47625.xlsx&quot;))
            {
                FileFormatInfo info = FileFormatUtil.DetectFileFormat(stream, &quot;1234&quot;);
                Assert.IsTrue(info.IsEncrypted);
               // Assert.IsFalse(info.IsPasswordValid);
            }
        }
```

### See Also

* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


