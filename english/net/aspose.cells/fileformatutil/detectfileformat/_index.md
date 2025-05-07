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
// Called: FileFormatInfo info = FileFormatUtil.DetectFileFormat(stream, "1234");
[Test]
        public void Method_String_()
        {
            using (Stream stream = File.OpenRead(Constants.sourcePath + "CellsNet47625.xlsx"))
            {
             //  FileFormatInfo info = FileFormatUtil.DetectFileFormat(stream, "test");
                Assert.IsTrue(FileFormatUtil.VerifyPassword(stream, "test"));
              //  Assert.IsTrue(info.IsPasswordValid);
            }
            using (Stream stream = File.OpenRead(Constants.sourcePath + "CellsNet47625.xlsx"))
            {
                FileFormatInfo info = FileFormatUtil.DetectFileFormat(stream, "1234");
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
// Called: Assert.AreEqual(FileFormatType.Excel2, FileFormatUtil.DetectFileFormat(Constants.sourcePath + @"App/Excel2/STAR614004CLNTASCDNL191202032235.XLS").FileFormatType);
[Test]
        public void Method_String_()
        {
            Assert.AreEqual(FileFormatType.Excel2, FileFormatUtil.DetectFileFormat(Constants.sourcePath + @"App/Excel2/STAR614004CLNTASCDNL191202032235.XLS").FileFormatType);
            Workbook workbook = new Workbook(Constants.sourcePath + @"App/Excel2/STAR614004CLNTASCDNL191202032235.XLS");
            Assert.AreEqual(21525, workbook.Worksheets[0].Cells["E3"].IntValue);

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
// Called: FileFormatUtil.DetectFileFormat(Constants.sourcePath + "CELLSNET46552.docx", "a").FileFormatType);
[Test]
        public void Method_String_()
        {
            Assert.AreEqual(FileFormatType.Xlsx,
                FileFormatUtil.DetectFileFormat(Constants.sourcePath + "CELLSNET46552.xlsx", "a").FileFormatType);
            Assert.AreEqual(FileFormatType.Docx,
                FileFormatUtil.DetectFileFormat(Constants.sourcePath + "CELLSNET46552.docx", "a").FileFormatType);
        }
```

### See Also

* class [FileFormatInfo](../../fileformatinfo/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


