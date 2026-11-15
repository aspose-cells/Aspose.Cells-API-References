---
title: Aspose::Cells::Rendering::SheetRender::ToImage method
linktitle: ToImage
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Rendering::SheetRender::ToImage method. Render certain page to a file in C++.'
type: docs
weight: 900
url: /tr/cpp/aspose.cells.rendering/sheetrender/toimage/
---
## SheetRender::ToImage(int32_t, const U16String\&) method


Render certain page to a file.

```cpp
void Aspose::Cells::Rendering::SheetRender::ToImage(int32_t pageIndex, const U16String &fileName)
```


| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | int32_t | indicate which page is to be converted |
| fileName | const U16String\& | filename of the output image |


## Examples


```cpp
Aspose::Cells::Startup();
//Aşağıdaki kod, ilk sayfanın ilk sayfasını png görüntüsü olarak dışa aktarır.

//görüntüler içeren kaynak dosyayı yükle.
Workbook wb(u"Book1.xlsx");

ImageOrPrintOptions imgOpt;

//Çıktı görüntü tipini ayarla.
imgOpt.SetImageType(ImageType::Png);

//İlk sayfayı renderla.
SheetRender sr(wb.GetWorksheets().Get(0), imgOpt);

//Sayfanın ilk sayfasını görüntüye çıkar.
U16String val =  u"output.png";
sr.ToImage(0, val);
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [SheetRender](../)
* Namespace [Aspose::Cells::Rendering](../../)
* Library [Aspose.Cells for C++](../../../)
## SheetRender::ToImage(int32_t, const char16_t*) method


Render certain page to a file.

```cpp
void Aspose::Cells::Rendering::SheetRender::ToImage(int32_t pageIndex, const char16_t *fileName)
```


| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | int32_t | indicate which page is to be converted |
| fileName | const char16_t* | filename of the output image |


## Examples


```cpp
Aspose::Cells::Startup();
//Aşağıdaki kod, ilk sayfanın ilk sayfasını png görüntüsü olarak dışa aktarır.

//görüntüler içeren kaynak dosyayı yükle.
Workbook wb(u"Book1.xlsx");

ImageOrPrintOptions imgOpt;

//Çıktı görüntü tipini ayarla.
imgOpt.SetImageType(ImageType::Png);

//İlk sayfayı renderla.
SheetRender sr(wb.GetWorksheets().Get(0), imgOpt);

//Sayfanın ilk sayfasını görüntüye çıkar.
sr.ToImage(0, u"output.png");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [SheetRender](../)
* Namespace [Aspose::Cells::Rendering](../../)
* Library [Aspose.Cells for C++](../../../)
## SheetRender::ToImage(int32_t) method


Render certain page to a stream.

```cpp
Vector<uint8_t> Aspose::Cells::Rendering::SheetRender::ToImage(int32_t pageIndex)
```


| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | int32_t | indicate which page is to be converted |

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [SheetRender](../)
* Namespace [Aspose::Cells::Rendering](../../)
* Library [Aspose.Cells for C++](../../../)
