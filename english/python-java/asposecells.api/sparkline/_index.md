---
title: "Sparkline Class"
linktitle: "Sparkline"
articleTitle: "Sparkline"
second_title: "Aspose.Cells for Python via Java"
description: "A sparkline represents a tiny chart or graphic in a worksheet cell that provides a visual representation of data."
type: docs
weight: 6270
url: /python-java/asposecells.api/sparkline/
---

## Sparkline class

A sparkline represents a tiny chart or graphic in a worksheet cell that provides a visual representation of data.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [DataRange](#datarange) | String | Represents the data range of the sparkline. |
| [Row](#row) | int | Gets the row index of the sparkline. |
| [Column](#column) | int | Gets the column index of the sparkline. |

## Methods

| Name | Description |
| --- | --- |
| [toImage](#toimage) | Converts a sparkline to an image. |
| [toImageBytes](#toimagebytes) | Converts a sparkline to an image. |

### Sparkline.DataRange property {#datarange}

Represents the data range of the sparkline.

**Type:** String

### Sparkline.Row property {#row}

Gets the row index of the sparkline.

**Type:** int

### Sparkline.Column property {#column}

Gets the column index of the sparkline.

**Type:** int

### toImage(fileName, options) (1 of 2) {#toimage}

Converts a sparkline to an image.

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | The image file name. |
| options | ImageOrPrintOptions | The image options |

---

### toImage(stream, options) (2 of 2) {#toimage-1}

Converts a sparkline to an image.

| Parameter | Type | Description |
| --- | --- | --- |
| stream | OutputStream | The image stream. |
| options | ImageOrPrintOptions | The image options. |

### toImageBytes(options) {#toimagebytes}

Converts a sparkline to an image.

| Parameter | Type | Description |
| --- | --- | --- |
| options | ImageOrPrintOptions | Addtional image creation options |

**Returns:** A byte array.

**Example:**

```python
import jpype
import asposecells
jpype.startJVM()
from asposecells.api import *

wb = Workbook("sparkline.xlsx")
sparkline = wb.getWorksheets().get(0).getSparklineGroupCollection().get(0).getSparklineCollection().get(0)
imgOptions = ImageOrPrintOptions()
imgOptions.setHorizontalResolution(200)
imgOptions.setVerticalResolution(300)
imgOptions.setImageFormat(ImageFormat.getJpeg())
with open("sparkline.jpeg", "wb") as w:
    content = sparkline.toImageBytes(imgOptions)
    w.write(content)

jpype.shutdownJVM()
```
