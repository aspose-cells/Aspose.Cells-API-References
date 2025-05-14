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
// Called: wb2.Save(savePath + "out.xlsx", SaveFormat.Xlsx);
public void Workbook_Method_Save()
{
    string filePath = Constants.JohnTest_PATH_SOURCE + @"NET44584/";
    Aspose.Cells.Workbook wb = new Aspose.Cells.Workbook(filePath + "Sample_1SpreadSheet.xlsx");
    Aspose.Cells.HtmlSaveOptions htmlSaveOptions = new HtmlSaveOptions();
    htmlSaveOptions.ExportDataOptions = HtmlExportDataOptions.All;
    htmlSaveOptions.LinkTargetType = HtmlLinkTargetType.Blank;

    string savePath = CreateFolder(filePath);
    wb.Save(savePath + "out.html", htmlSaveOptions);

    Aspose.Cells.LoadOptions htmlLoadOptions = new Aspose.Cells.HtmlLoadOptions(LoadFormat.Html);
    Aspose.Cells.Workbook wb2 = new Workbook(savePath + "out.html", htmlLoadOptions);
    wb2.Save(savePath + "out.xlsx", SaveFormat.Xlsx);
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
// Called: workbook.Save(Constants.destPath + " testInsertRows.xlsx");
public void Workbook_Method_Save()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    Cells cells = workbook.Worksheets[0].Cells;
    cells.InsertRows(1, 2);

    CheckInsertRows_Formual_002(workbook);
    workbook.Save(Constants.destPath + " testInsertRows.xls");
    workbook = new Workbook(Constants.destPath + " testInsertRows.xls");
    CheckInsertRows_Formual_002(workbook);
    workbook.Save(Constants.destPath + " testInsertRows.xlsx");
    workbook = new Workbook(Constants.destPath + " testInsertRows.xlsx");
    CheckInsertRows_Formual_002(workbook);
    workbook.Save(Constants.destPath + " testInsertRows.xml", SaveFormat.SpreadsheetML);
    workbook = new Workbook(Constants.destPath + " testInsertRows.xml");
    CheckInsertRows_Formual_002(workbook);
    workbook.Save(Constants.destPath + " testInsertRows.xls");
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
// Called: wb.Save(CreateFolder(filePath) + "out.html", options);
public void Workbook_Method_Save()
{
    string filePath = Constants.JohnTest_PATH_SOURCE + @"NET45331/";
    Workbook wb = new Workbook(filePath + "Input.xls");
    HtmlSaveOptions options = new HtmlSaveOptions();
    options.IsExportComments = true;
    wb.Save(CreateFolder(filePath) + "out.html", options);
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
public void Workbook_Method_Save()
{
    string fileName = "NOA.xls";
    string fileSrc = Constants.MhtmlPath + fileName;
    Workbook wb = new Workbook(fileSrc);
    Stream s = new MemoryStream();
    wb.Save(s, SaveFormat.MHtml);
    s.Seek(0, SeekOrigin.Begin);
    string fileDestMht = _destFilesPath + "SaveToStream4" + ".mht";
          
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


