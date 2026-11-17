---
title: "Clase SheetRender"
linktitle: "SheetRender"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "Clase SheetRender. Encapsula el objeto que representa sheetrender en Go."
type: docs
weight: 200
url: /es/go-cpp/sheetrender/
---

## SheetRender class

Represents a worksheet render which can render worksheet to various images such as (BMP, PNG, JPEG, TIFF..)The constructor of this class , must be used after modification of pagesetup, cell style.

```go

type SheetRender struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |
| [NewSheetRender](./newsheetrender/) | La construcción de SheetRender necesita worksheet e ImageOrPrintOptions como parámetros. |

## Methods

| Method | Description |
| --- | --- |
| [IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
| [GetPageCount](./getpagecount/) | Obtiene el recuento total de páginas de la hoja de cálculo actual. |
| [GetPageScale](./getpagescale/) | Obtiene la escala de página calculada de la hoja. Devuelve la escala establecida si PageSetup.Zoom está configurado. De lo contrario, devuelve la escala calculada según PageSetup.FitToPagesWide y PageSetup.FitToPagesTall. |
| [GetPageSizeInch](./getpagesizeinch/) | Obtenga el tamaño de página en pulgadas de la imagen de salida. |
| [ToImage_Int_String](./toimage_int_string/) | Renderiza una página determinada a un archivo. |
| [ToImage_Int](./toimage_int/) | Renderiza una página determinada a un stream. |
| [ToTiff](./totiff/) | Renderiza toda la hoja de cálculo como imagen Tiff a un flujo. |
| [ToTiff_String](./totiff_string/) | Renderiza toda la hoja de cálculo como imagen Tiff a un archivo. |
| [Dispose](./dispose/) | Libera los recursos creados y utilizados para el renderizado. |
