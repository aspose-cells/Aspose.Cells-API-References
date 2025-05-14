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
// Called: workbook = new Workbook(_destFilesPath + "CELLSNET49301.mht");
public void Workbook_Constructor()
{
    Workbook workbook = new Workbook(Constants.MhtmlPath + "example.xlsx");
    workbook.Save(_destFilesPath + "CELLSNET49301.mht");
    workbook = new Workbook(_destFilesPath + "CELLSNET49301.mht");
    Assert.AreEqual(2, workbook.Worksheets.Count);
    CheckWorksheet49300_1(workbook.Worksheets[0]);
    CheckWorksheet49300_1(workbook.Worksheets[1]);
    workbook = new Workbook(Constants.MhtmlPath + "example.xlsx");
    workbook = Util.ReSave(workbook, SaveFormat.MHtml);
    Assert.AreEqual(2, workbook.Worksheets.Count);
    CheckWorksheet49300_1(workbook.Worksheets[0]);
    CheckWorksheet49300_1(workbook.Worksheets[1]);
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
// Called: Workbook wb = new Workbook(
public void Workbook_Constructor()
{
    Workbook wb = new Workbook(
        Constants.batchPath + "calculate\\FormulaCalc_Table.xlsb",
        new LoadOptions()
        { LightCellsDataHandler = new LightCellsDataHandlerNone() });
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


