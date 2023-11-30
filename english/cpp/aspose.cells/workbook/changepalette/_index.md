---
title: Aspose::Cells::Workbook::ChangePalette method
linktitle: ChangePalette
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Workbook::ChangePalette method. Changes the palette for the spreadsheet in the specified index in C++.'
type: docs
weight: 2700
url: /cpp/aspose.cells/workbook/changepalette/
---
## Workbook::ChangePalette method


Changes the palette for the spreadsheet in the specified index.

```cpp
void Aspose::Cells::Workbook::ChangePalette(const Aspose::Cells::Color &color, int32_t index)
```


| Parameter | Type | Description |
| --- | --- | --- |
| color | const Aspose::Cells::Color\& | [Color](../../color/) structure. |
| index | int32_t | Palette index, 0 - 55. |
## Remarks



The palette has 56 entries, each represented by an RGB value.

If you set a color which is not in the palette, it will not take effect.

So if you want to set a custom color, please change the palette at first.

The following is the standard color palette.

<table><tr><th>Color</th><th>Red </th><th>Green </th><th>Blue  </th></tr><tr><td>Black </td><td>0 </td><td>0 </td><td>0  </td></tr><tr><td>White </td><td>255 </td><td>255 </td><td>255  </td></tr><tr><td>Red </td><td>255 </td><td>0 </td><td>0  </td></tr><tr><td>Lime </td><td>0 </td><td>255 </td><td>0  </td></tr><tr><td>Blue </td><td>0 </td><td>0 </td><td>255  </td></tr><tr><td>Yellow </td><td>255 </td><td>255 </td><td>0  </td></tr><tr><td>Magenta </td><td>255 </td><td>0 </td><td>255  </td></tr><tr><td>Cyan </td><td>0 </td><td>255 </td><td>255  </td></tr><tr><td>Maroon </td><td>128 </td><td>0 </td><td>0  </td></tr><tr><td>Green </td><td>0 </td><td>128 </td><td>0  </td></tr><tr><td>Navy </td><td>0 </td><td>0 </td><td>128  </td></tr><tr><td>Olive </td><td>128 </td><td>128 </td><td>0  </td></tr><tr><td>Purple </td><td>128 </td><td>0 </td><td>128  </td></tr><tr><td>Teal </td><td>0 </td><td>128 </td><td>128  </td></tr><tr><td>Silver </td><td>192 </td><td>192 </td><td>192  </td></tr><tr><td>Gray </td><td>128 </td><td>128 </td><td>128  </td></tr><tr><td>Color17 </td><td>153 </td><td>153 </td><td>255  </td></tr><tr><td>Color18 </td><td>153 </td><td>51 </td><td>102  </td></tr><tr><td>Color19 </td><td>255 </td><td>255 </td><td>204  </td></tr><tr><td>Color20 </td><td>204 </td><td>255 </td><td>255  </td></tr><tr><td>Color21 </td><td>102 </td><td>0 </td><td>102  </td></tr><tr><td>Color22 </td><td>255 </td><td>128 </td><td>128  </td></tr><tr><td>Color23 </td><td>0 </td><td>102 </td><td>204  </td></tr><tr><td>Color24 </td><td>204 </td><td>204 </td><td>255  </td></tr><tr><td>Color25 </td><td>0 </td><td>0 </td><td>128  </td></tr><tr><td>Color26 </td><td>255 </td><td>0 </td><td>255  </td></tr><tr><td>Color27 </td><td>255 </td><td>255 </td><td>0  </td></tr><tr><td>Color28 </td><td>0 </td><td>255 </td><td>255  </td></tr><tr><td>Color29 </td><td>128 </td><td>0 </td><td>128  </td></tr><tr><td>Color30 </td><td>128 </td><td>0 </td><td>0  </td></tr><tr><td>Color31 </td><td>0 </td><td>128 </td><td>128  </td></tr><tr><td>Color32 </td><td>0 </td><td>0 </td><td>255  </td></tr><tr><td>Color33 </td><td>0 </td><td>204 </td><td>255  </td></tr><tr><td>Color34 </td><td>204 </td><td>255 </td><td>255  </td></tr><tr><td>Color35 </td><td>204 </td><td>255 </td><td>204  </td></tr><tr><td>Color36 </td><td>255 </td><td>255 </td><td>153  </td></tr><tr><td>Color37 </td><td>153 </td><td>204 </td><td>255  </td></tr><tr><td>Color38 </td><td>255 </td><td>153 </td><td>204  </td></tr><tr><td>Color39 </td><td>204 </td><td>153 </td><td>255  </td></tr><tr><td>Color40 </td><td>255 </td><td>204 </td><td>153  </td></tr><tr><td>Color41 </td><td>51 </td><td>102 </td><td>255  </td></tr><tr><td>Color42 </td><td>51 </td><td>204 </td><td>204  </td></tr><tr><td>Color43 </td><td>153 </td><td>204 </td><td>0  </td></tr><tr><td>Color44 </td><td>255 </td><td>204 </td><td>0  </td></tr><tr><td>Color45 </td><td>255 </td><td>153 </td><td>0  </td></tr><tr><td>Color46 </td><td>255 </td><td>102 </td><td>0  </td></tr><tr><td>Color47 </td><td>102 </td><td>102 </td><td>153  </td></tr><tr><td>Color48 </td><td>150 </td><td>150 </td><td>150  </td></tr><tr><td>Color49 </td><td>0 </td><td>51 </td><td>102  </td></tr><tr><td>Color50 </td><td>51 </td><td>153 </td><td>102  </td></tr><tr><td>Color51 </td><td>0 </td><td>51 </td><td>0  </td></tr><tr><td>Color52 </td><td>51 </td><td>51 </td><td>0  </td></tr><tr><td>Color53 </td><td>153 </td><td>51 </td><td>0  </td></tr><tr><td>Color54 </td><td>153 </td><td>51 </td><td>102  </td></tr><tr><td>Color55 </td><td>51 </td><td>51 </td><td>153  </td></tr><tr><td>Color56 </td><td>51 </td><td>51 </td><td>51  </td></tr></table>
## See Also

* Class [Vector](../../vector/)
* Class [Workbook](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
