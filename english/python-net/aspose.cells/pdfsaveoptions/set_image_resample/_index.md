---
title: set_image_resample method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 20
url: /python-net/aspose.cells/pdfsaveoptions/set_image_resample/
is_root: false
---

## set_image_resample(desired_ppi, jpeg_quality) {#int-int}

Sets desired PPI(pixels per inch) of resample images and jpeg quality.  
All images will be converted to JPEG with the specified quality setting, 
and images that are greater than the specified PPI (pixels per inch) will be resampled.



```python
def set_image_resample(self, desired_ppi, jpeg_quality):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| desired_ppi | int | Desired pixels per inch. 220 high quality. 150 screen quality. 96 email quality. |
| jpeg_quality | int | 0 - 100% JPEG quality. |



### See Also
* module [aspose.cells](../../)
* class [PdfSaveOptions](/cells/python-net/aspose.cells/pdfsaveoptions)
