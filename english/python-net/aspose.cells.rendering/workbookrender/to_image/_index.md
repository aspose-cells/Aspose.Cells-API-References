---
title: to_image method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 40
url: /python-net/aspose.cells.rendering/workbookrender/to_image/
is_root: false
---

## to_image(stream) {#io.RawIOBase}

Render whole workbook as Tiff Image to stream.



```python
def to_image(self, stream):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| stream | io.RawIOBase | the stream of the output image |


## to_image(filename) {#str}

Render whole workbook as Tiff Image to a file.



```python
def to_image(self, filename):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| filename | str | the filename of the output image |


## to_image(page_index, file_name) {#int-str}

Render certain page to a file.



```python
def to_image(self, page_index, file_name):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| page_index | int | indicate which page is to be converted |
| file_name | str | filename of the output image |


## to_image(page_index, stream) {#int-io.RawIOBase}

Render certain page to a stream.



```python
def to_image(self, page_index, stream):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| page_index | int | indicate which page is to be converted |
| stream | io.RawIOBase | the stream of the output image |



### See Also
* module [aspose.cells.rendering](../../)
* class [WorkbookRender](/cells/python-net/aspose.cells.rendering/workbookrender)
