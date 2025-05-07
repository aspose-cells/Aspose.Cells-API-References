---
title: Workbook.Workbook
second_title: Aspose.Cells for .NET API Reference
description: Workbook constructor. Initializes a new instance of the Workbook class
type: docs
url: /net/aspose.cells/workbook/workbook/
---
## Workbook() {#constructor}

Initializes a new instance of the [`Workbook`](../) class.

```csharp
public Workbook()
```

### Remarks

The default file format type is Xlsx. If you want to create other types of files, please use Workbook(FileFormatType).

### Examples

The following code shows how to use the Workbook constructor to create and initialize a new instance of the class.

```csharp
[C#]

Workbook workbook = new Workbook();
		

[Visual Basic]

Dim workbook as Workbook = new Workbook()
		
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Workbook(FileFormatType) {#constructor_1}

Initializes a new instance of the [`Workbook`](../) class.

```csharp
public Workbook(FileFormatType fileFormatType)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fileFormatType | FileFormatType | The new file format. |

### Remarks

The default file format type is Excel97To2003.

### Examples

The following code shows how to use the Workbook constructor to create and initialize a new instance of the class with various file format type.

```csharp
[C#]

Workbook workbook = new Workbook(FileFormatType.Xlsx);
		

[Visual Basic]

Dim workbook as Workbook = new Workbook(FileFormatType.Xlsx)
		
```

### See Also

* enum [FileFormatType](../../fileformattype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Workbook(string) {#constructor_4}

Initializes a new instance of the [`Workbook`](../) class and open a file.

```csharp
public Workbook(string file)
```

| Parameter | Type | Description |
| --- | --- | --- |
| file | String | The file name. |

### Examples

```csharp
// Called: workbook = new Workbook(Constants.sourcePath + "insertDelete\\testformual2.xls");
[Test, Ignore("Not ready to test this yet")]
        public void Workbook_Constructor()
        {
            caseName = "testCopyRow_Formual_001";
            Workbook workbook = new Workbook();
            workbook = new Workbook(Constants.sourcePath + "insertDelete\\testformual2.xls");
            Cells cells = workbook.Worksheets[0].Cells;
            cells.CopyRow(cells, 1, 0);

            checkCopyRow_Formual_001(workbook);
            workbook.Save(Constants.destPath + "testCopyRow.xls");
            workbook = new Workbook(Constants.destPath + "testCopyRow.xls");
            checkCopyRow_Formual_001(workbook);
            workbook.Save(Constants.destPath + "testCopyRow.xlsx");
            workbook = new Workbook(Constants.destPath + "testCopyRow.xlsx");
            checkCopyRow_Formual_001(workbook);
            workbook.Save(Constants.destPath + "testCopyRow.xml", SaveFormat.SpreadsheetML);
            workbook = new Workbook(Constants.destPath + "testCopyRow.xml");
            checkCopyRow_Formual_001(workbook);
            workbook.Save(Constants.destPath + "testCopyRow.xls");
        }
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Workbook(Stream) {#constructor_2}

Initializes a new instance of the [`Workbook`](../) class and open a stream.

```csharp
public Workbook(Stream stream)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | The stream. |

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Workbook(string, LoadOptions) {#constructor_5}

Initializes a new instance of the [`Workbook`](../) class and open a file.

```csharp
public Workbook(string file, LoadOptions loadOptions)
```

| Parameter | Type | Description |
| --- | --- | --- |
| file | String | The file name. |
| loadOptions | LoadOptions | The load options |

### Examples

```csharp
// Called: Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET46296.xlsx", loadOptions);
[Test]
        public void Workbook_Constructor()
        {
            AutoFitterOptions options = new AutoFitterOptions();
            options.OnlyAuto = true;
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.AutoFitterOptions = options;
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET46296.xlsx", loadOptions);
            Assert.AreEqual(76.5, workbook.Worksheets[0].Cells.GetRowHeight(12));
        }
```

### See Also

* class [LoadOptions](../../loadoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Workbook(Stream, LoadOptions) {#constructor_3}

Initializes a new instance of the [`Workbook`](../) class and open stream.

```csharp
public Workbook(Stream stream, LoadOptions loadOptions)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | The stream. |
| loadOptions | LoadOptions | The load options |

### See Also

* class [LoadOptions](../../loadoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


