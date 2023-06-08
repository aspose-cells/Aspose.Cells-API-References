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


