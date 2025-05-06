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
// Called: Workbook workbook = new Workbook(Constants.PivotTableSourcePath + &amp;quot;CellsNet57038.xlsx&amp;quot;);
[Test]
        public void Workbook_Constructor()
        {

            Workbook workbook = new Workbook(Constants.PivotTableSourcePath + &quot;CellsNet57038.xlsx&quot;);
            //CELLSNET-57042
            workbook.Settings.PropertiesFollowChartPoint = true;
            // Save the workbook
            workbook.Save(Constants.PivotTableDestPath + &quot;CellsNet57038.xlsx&quot;);
            bool c = ManualFileUtil.ManualCheckStringInZip(Constants.PivotTableDestPath + @&quot;CellsNet57038.xlsx&quot;, &quot;xl/pivotTables/pivotTable1.xml&quot;, new string[] { &quot;e=\&quot;0\&quot;&quot; }, true);
            Assert.IsTrue(c);
            workbook = new Workbook(Constants.PivotTableDestPath + &quot;CellsNet57038.xlsx&quot;);
            workbook.Save(Constants.PivotTableDestPath + &quot;CellsNet57038.xlsb&quot;);
            workbook = new Workbook(Constants.PivotTableDestPath + &quot;CellsNet57038.xlsb&quot;);
            Assert.IsTrue(workbook.Settings.PropertiesFollowChartPoint);

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
// Called: var workbook = new Workbook(filePath + &amp;quot;386.mht&amp;quot;, ldps);
[Test]
        public void Workbook_Constructor()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;NET46494/&quot;;

            Workbook wb = new Workbook(filePath + &quot;job-search-k-ARtitle.xls (ARtitle.xls)-h-ARtitle.htm&quot;);
            //return;

            HtmlLoadOptions ldps = new HtmlLoadOptions(LoadFormat.MHtml);
            var workbook = new Workbook(filePath + &quot;386.mht&quot;, ldps);

            Assert.Greater(workbook.Worksheets[0].Cells[&quot;D6&quot;].StringValue.Length, 100);
            workbook.Save(CreateFolder(filePath) + &quot;out.xlsx&quot;, SaveFormat.Xlsx);
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


