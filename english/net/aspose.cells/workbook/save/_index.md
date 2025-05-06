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
// Called: workbook.Save(Constants.destPath + &amp;quot;testRangeCopy.xml&amp;quot;, SaveFormat.SpreadsheetML);
[Test]
        public void Method_SaveFormat_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;Copy\\testPatternSetting.xls&quot;);
            Cells cells = workbook.Worksheets[0].Cells;
            Aspose.Cells.Range rangeSrc = cells.CreateRange(0, 0, 12, 6);
            Aspose.Cells.Range rangeDest = cells.CreateRange(16, 0, 12, 6);
            rangeDest.Copy(rangeSrc);

            checkRangeCopy_PatternSetting(workbook);
            workbook.Save(Constants.destPath + &quot;testRangeCopy.xls&quot;);
            workbook = new Workbook(Constants.destPath + &quot;testRangeCopy.xls&quot;);
            checkRangeCopy_PatternSetting(workbook);
            workbook.Save(Constants.destPath + &quot;testRangeCopy.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;testRangeCopy.xlsx&quot;);
            checkRangeCopy_PatternSetting(workbook);
            workbook.Save(Constants.destPath + &quot;testRangeCopy.xml&quot;, SaveFormat.SpreadsheetML);
            workbook = new Workbook(Constants.destPath + &quot;testRangeCopy.xml&quot;);
            checkRangeCopy_PatternSetting(workbook);
            workbook.Save(Constants.destPath + &quot;testRangeCopy.xls&quot;);
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
// Called: l.Save(Constants.PivotTableDestPath + &amp;quot;CELLSNET43580.pdf&amp;quot;);
[Test]
        public void Method_String_()
        {
            Workbook l = new Aspose.Cells.Workbook(Constants.PivotTableSourcePath + &quot;CELLSNET43580.xlsx&quot;);
            l.CalculateFormula();
            l.Save(Constants.PivotTableDestPath + &quot;CELLSNET43580.pdf&quot;);
            Assert.IsTrue(Util.CompareColor(Color.FromArgb(79, 129, 189), l.Worksheets[1].Cells[&quot;B3&quot;].GetStyle().ForegroundColor));
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
// Called: workbook.Save(Constants.destPath + &amp;quot;CELLSNET54208.xlsx&amp;quot;, ooxmlSaveOptions);
[Test]
        public void Method_SaveOptions_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET-54208.xlsx&quot;);
            OoxmlSaveOptions ooxmlSaveOptions = new OoxmlSaveOptions();
            workbook.Save(Constants.destPath + &quot;CELLSNET54208.xlsx&quot;, ooxmlSaveOptions);
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
            string fileName = &quot;_vip_fr_DefaultReport.xls&quot;;
            string fileSrc = Constants.MhtmlPath + fileName;
            Workbook wb = new Workbook(fileSrc);
            Stream s = new MemoryStream();
            wb.Save(s, SaveFormat.MHtml);
            s.Seek(0, SeekOrigin.Begin);

            string fileDestMht = _destFilesPath + &quot;SaveToStream1&quot; + &quot;.mht&quot;;
            StreamReader sr = new StreamReader(s);
            StreamWriter sw = new StreamWriter(fileDestMht,false, Encoding.UTF8);
            sw.Write(sr.ReadToEnd());
            sw.Flush();
            sw.Close();
            sr.Close();

            string fileDest = fileDestMht + &quot;.net.xls&quot;;
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


