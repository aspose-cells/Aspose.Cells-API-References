---
title: Workbook.Save
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Saves the workbook to the disk
type: docs
url: /net/aspose.cells/workbook/save/
---
## Save(string, SaveFormat) {#save_3}

Saves the workbook to the disk.

```csharp
public void Save(string fileName, SaveFormat saveFormat)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | The file name. |
| saveFormat | SaveFormat | The save format type. |

### Examples

```csharp
// Called: workbook.Save(Constants.destPath + "testRangeCopyData.xml", SaveFormat.SpreadsheetML);
[Test, Ignore("Not ready to test this yet")]
        public void Method_SaveFormat_()
        {
            caseName = "testRangeCopyData_ConditionalFormatting";
            Workbook workbook = new Workbook(Constants.sourcePath + "copy\\testConditionalFormatting.xls");
            Worksheet sheetSrc = workbook.Worksheets[0];
            Cells cellsSrc = sheetSrc.Cells;
            Worksheet sheetDest = workbook.Worksheets[workbook.Worksheets.Add()];
            sheetDest.Name = "sheetDest";
            Cells cellsDest = sheetDest.Cells;
            Aspose.Cells.Range rangeSrc = cellsSrc.CreateRange(0, 0, 9, 7);
            Aspose.Cells.Range rangeDest = cellsDest.CreateRange(0, 0, 9, 7);
            rangeDest.CopyData(rangeSrc);

            checkRangeCopyData_ConditionalFormatting(workbook);
            workbook.Save(Constants.destPath + "testRangeCopyData.xls");
            workbook = new Workbook(Constants.destPath + "testRangeCopyData.xls");
            checkRangeCopyData_ConditionalFormatting(workbook);
            workbook.Save(Constants.destPath + "testRangeCopyData.xlsx");
            workbook = new Workbook(Constants.destPath + "testRangeCopyData.xlsx");
            checkRangeCopyData_ConditionalFormatting(workbook);
            workbook.Save(Constants.destPath + "testRangeCopyData.xml", SaveFormat.SpreadsheetML);
            workbook = new Workbook(Constants.destPath + "testRangeCopyData.xml");
            checkRangeCopyData_ConditionalFormatting(workbook);
            workbook.Save(Constants.destPath + "testRangeCopyData.xls");
        }
```

### See Also

* enum [SaveFormat](../../saveformat/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(string) {#save_2}

Save the workbook to the disk.

```csharp
public void Save(string fileName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String |  |

### Examples

```csharp
// Called: workbook.Save(Constants.destPath + "testCopyRows.xls");
[Test]
        public void Method_String_()
        {
            caseName = "testCopyRows_Formual_004";
            Workbook workbook = new Workbook();
            workbook = new Workbook(Constants.sourcePath + "Cells\\deleteColumn_002.xls");
            Cells cellsSrc = workbook.Worksheets[0].Cells;
            Worksheet sheetDest = workbook.Worksheets[workbook.Worksheets.Add()];
            sheetDest.Name = "sheetDest";
            Cells cellsDest = sheetDest.Cells;
            cellsDest.CopyRows(cellsSrc, 0, 1, 5);

            checkCopyRows_Formual_004(workbook);
            workbook.Save(Constants.destPath + "testCopyRows.xls");
            workbook = new Workbook(Constants.destPath + "testCopyRows.xls");
            checkCopyRows_Formual_004(workbook);
            workbook.Save(Constants.destPath + "testCopyRows.xlsx");
            workbook = new Workbook(Constants.destPath + "testCopyRows.xlsx");
            checkCopyRows_Formual_004(workbook);
            workbook.Save(Constants.destPath + "testCopyRows.xml", SaveFormat.SpreadsheetML);
            workbook = new Workbook(Constants.destPath + "testCopyRows.xml");
            checkCopyRows_Formual_004(workbook);
            workbook.Save(Constants.destPath + "testCopyRows.xls");
        }
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(string, SaveOptions) {#save_4}

Saves the workbook to the disk.

```csharp
public void Save(string fileName, SaveOptions saveOptions)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | The file name. |
| saveOptions | SaveOptions | The save options. |

### Examples

```csharp
// Called: workbook.Save(Constants.destPath + "CellsNet46737.ods", saveOptions);
[Test]
        public void Method_SaveOptions_()
        {
            Style style = null;
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet46737.xlsx");
            OdsSaveOptions saveOptions = new OdsSaveOptions();
            saveOptions.GeneratorType = Aspose.Cells.Ods.OdsGeneratorType.LibreOffice;
            
            workbook.Save(Constants.destPath + "CellsNet46737.ods", saveOptions);
            workbook = new Workbook(Constants.destPath + "CellsNet46737.ods");
            style = workbook.Worksheets[0].Cells["B2"].GetStyle();
            Assert.AreEqual(style.Borders[BorderType.RightBorder].LineStyle, CellBorderType.Medium);
            style = workbook.Worksheets[0].Cells["B4"].GetStyle();
            Assert.AreEqual(style.Borders[BorderType.RightBorder].LineStyle, CellBorderType.Thick);
            style = workbook.Worksheets[0].Cells["B7"].GetStyle();
            Assert.AreEqual(style.Borders[BorderType.RightBorder].LineStyle, CellBorderType.Double);
            workbook.Save(Constants.destPath + "CellsNet46737dest.xlsx");
            workbook = new Workbook(Constants.destPath + "CellsNet46737dest.xlsx");
            style = workbook.Worksheets[0].Cells["B2"].GetStyle();
            Assert.AreEqual(style.Borders[BorderType.RightBorder].LineStyle, CellBorderType.Medium);
            style = workbook.Worksheets[0].Cells["B4"].GetStyle();
            Assert.AreEqual(style.Borders[BorderType.RightBorder].LineStyle, CellBorderType.Thick);
            style = workbook.Worksheets[0].Cells["B7"].GetStyle();
            Assert.AreEqual(style.Borders[BorderType.RightBorder].LineStyle, CellBorderType.Double);
        }
```

### See Also

* class [SaveOptions](../../saveoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(Stream, SaveFormat) {#save}

Saves the workbook to the stream.

```csharp
public void Save(Stream stream, SaveFormat saveFormat)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | The file stream. |
| saveFormat | SaveFormat | The save file format type. |

### Examples

```csharp
// Called: wb.Save(s, SaveFormat.MHtml);
[Test]
        public void Method_SaveFormat_()
        {
            string fileName = "Dashboard.xls";
            string fileSrc = Constants.MhtmlPath + fileName;
            Workbook wb = new Workbook(fileSrc);
            Stream s = new MemoryStream();
            wb.Save(s, SaveFormat.MHtml);
            s.Seek(0, SeekOrigin.Begin);
            string fileDestMht = _destFilesPath + "SaveToStream3" + ".mht";
         
            StreamReader sr = new StreamReader(s);
            StreamWriter sw = new StreamWriter(fileDestMht, false, Encoding.UTF8);
            sw.Write(sr.ReadToEnd());
            sw.Flush();
            sw.Close();
            sr.Close();

            string fileDest = fileDestMht + ".net.xls";
            Workbook workbook = new Workbook(fileDestMht);
            workbook.Save(fileDest);
            CompareOption option = InitCompareOption();
            CompareAction.Compare(fileSrc, fileDest, option);
        }
```

### See Also

* enum [SaveFormat](../../saveformat/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(Stream, SaveOptions) {#save_1}

Saves the workbook to the stream.

```csharp
public void Save(Stream stream, SaveOptions saveOptions)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | The file stream. |
| saveOptions | SaveOptions | The save options. |

### See Also

* class [SaveOptions](../../saveoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(HttpResponse, string, ContentDisposition, SaveOptions) {#save_5}

Creates the result spreadsheet and transfer it to the client then open it in the browser or MS Workbook.

```csharp
public void Save(HttpResponse response, string fileName, ContentDisposition contentDisposition, 
    SaveOptions saveOptions)
```

| Parameter | Type | Description |
| --- | --- | --- |
| response | HttpResponse | Response object to return the spreadsheet to client. |
| fileName | String | The name of created file. |
| contentDisposition | ContentDisposition | The content disposition type. |
| saveOptions | SaveOptions | The save options. |

### See Also

* enum [ContentDisposition](../../contentdisposition/)
* class [SaveOptions](../../saveoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(HttpResponse, string, ContentDisposition, SaveOptions, bool) {#save_6}

Creates the result spreadsheet and transfer it to the client then open it in the browser or MS Workbook.

```csharp
public void Save(HttpResponse response, string fileName, ContentDisposition contentDisposition, 
    SaveOptions saveOptions, bool enableHttpCompression)
```

| Parameter | Type | Description |
| --- | --- | --- |
| response | HttpResponse | Response object to return the spreadsheet to client. |
| fileName | String | The name of created file. |
| contentDisposition | ContentDisposition | The content disposition type. |
| saveOptions | SaveOptions | The save options. |
| enableHttpCompression | Boolean | whether http compression is to be used |

### See Also

* enum [ContentDisposition](../../contentdisposition/)
* class [SaveOptions](../../saveoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


