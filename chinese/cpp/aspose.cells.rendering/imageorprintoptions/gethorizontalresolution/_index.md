---
title: Aspose::Cells::Rendering::ImageOrPrintOptions::GetHorizontalResolution method
linktitle: GetHorizontalResolution
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Rendering::ImageOrPrintOptions::GetHorizontalResolution method. Gets or sets the horizontal resolution for generated images, in dots per inch in C++.'
type: docs
weight: 800
url: /zh/cpp/aspose.cells.rendering/imageorprintoptions/gethorizontalresolution/
---
## ImageOrPrintOptions::GetHorizontalResolution method


Gets or sets the horizontal resolution for generated images, in dots per inch.

```cpp
int32_t Aspose::Cells::Rendering::ImageOrPrintOptions::GetHorizontalResolution()
```

## Remarks


The default value is 96.

Setting HorizontalResolution and VerticalResolution effects the width and height of the output image in pixels.

## Examples


```cpp
Aspose::Cells::Startup();
//          以下代码将分辨率设置为 192，生成图像的宽度和高度是原来的两倍。
//          分辨率保持默认值 96 的那个。
Workbook wb(u"Book1.xlsx");

ImageOrPrintOptions opts;

//设置输出图像类型：png。
opts.SetImageType(ImageType::Png);

//将分辨率设置为 192。
opts.SetHorizontalResolution(192);
opts.SetVerticalResolution(192);

//将工作表页面渲染为图像。
SheetRender sr(wb.GetWorksheets().Get(0), opts);
sr.ToImage(0, u"Sheet_Page1.png");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [ImageOrPrintOptions](../)
* Namespace [Aspose::Cells::Rendering](../../)
* Library [Aspose.Cells for C++](../../../)
