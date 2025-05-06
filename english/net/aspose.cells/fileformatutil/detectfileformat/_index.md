---
title: FileFormatUtil.DetectFileFormat
second_title: Aspose.Cells for .NET API Reference
description: FileFormatUtil method. Detects and returns the information about a format of an excel stored in a stream
type: docs
url: /net/aspose.cells/fileformatutil/detectfileformat/
---
## DetectFileFormat(Stream) {#detectfileformat}

Detects and returns the information about a format of an excel stored in a stream.

```csharp
public static FileFormatInfo DetectFileFormat(Stream stream)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream |  |

### Return Value

A [`FileFormatInfo`](../../fileformatinfo/) object that contains the detected information.

### See Also

* class [FileFormatInfo](../../fileformatinfo/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DetectFileFormat(Stream, string) {#detectfileformat_1}

Detects and returns the information about a format of an excel stored in a stream.

```csharp
public static FileFormatInfo DetectFileFormat(Stream stream, string password)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream |  |
| password | String | The password for encrypted ooxml files. |

### Return Value

A [`FileFormatInfo`](../../fileformatinfo/) object that contains the detected information.

### Examples

```csharp
// Called: FileFormatInfo info = FileFormatUtil.DetectFileFormat(stream, &amp;quot;1234&amp;quot;);
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

* class [FileFormatInfo](../../fileformatinfo/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DetectFileFormat(string) {#detectfileformat_2}

Detects and returns the information about a format of an excel stored in a file.

```csharp
public static FileFormatInfo DetectFileFormat(string filePath)
```

| Parameter | Type | Description |
| --- | --- | --- |
| filePath | String | The file path. |

### Return Value

A [`FileFormatInfo`](../../fileformatinfo/) object that contains the detected information.

### Examples

```csharp
// Called: Assert.AreEqual(FileFormatUtil.DetectFileFormat(Constants.sourcePath + &amp;quot;ExchangeRates1-8.2012.xls&amp;quot;).FileFormatType, FileFormatType.Excel95);
[Test]
        public void Method_String_()
        {
            Assert.AreEqual(FileFormatUtil.DetectFileFormat(Constants.sourcePath + &quot;ExchangeRates1-8.2012.xls&quot;).FileFormatType, FileFormatType.Excel95);
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;ExchangeRates1-8.2012.xls&quot;);
            workbook.Save(Constants.destPath + &quot;CellsNet41038.xls&quot;);
        }
```

### See Also

* class [FileFormatInfo](../../fileformatinfo/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DetectFileFormat(string, string) {#detectfileformat_3}

Detects and returns the information about a format of an excel stored in a file.

```csharp
public static FileFormatInfo DetectFileFormat(string filePath, string password)
```

| Parameter | Type | Description |
| --- | --- | --- |
| filePath | String | The file path. |
| password | String | The password for encrypted ooxml files. |

### Return Value

A [`FileFormatInfo`](../../fileformatinfo/) object that contains the detected information.

### Examples

```csharp
// Called: FileFormatUtil.DetectFileFormat(Constants.sourcePath + &amp;quot;CELLSNET46552.docx&amp;quot;, &amp;quot;a&amp;quot;).FileFormatType);
[Test]
        public void Method_String_()
        {
            Assert.AreEqual(FileFormatType.Xlsx,
                FileFormatUtil.DetectFileFormat(Constants.sourcePath + &quot;CELLSNET46552.xlsx&quot;, &quot;a&quot;).FileFormatType);
            Assert.AreEqual(FileFormatType.Docx,
                FileFormatUtil.DetectFileFormat(Constants.sourcePath + &quot;CELLSNET46552.docx&quot;, &quot;a&quot;).FileFormatType);
        }
```

### See Also

* class [FileFormatInfo](../../fileformatinfo/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


