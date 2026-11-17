---
title: "Clase WorkbookRender"
linktitle: "WorkbookRender"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "Clase WorkbookRender. Encapsula el objeto que representa workbookrender en Go."
type: docs
weight: 200
url: /es/go-cpp/workbookrender/
---

## WorkbookRender class

Represents a Workbook render.The constructor of this class , must be used after modification of pagesetup, cell style.

```go

type WorkbookRender struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |
| [NewWorkbookRender](./newworkbookrender/) | La construcción de WorkbookRender |

## Methods

| Method | Description |
| --- | --- |
| [IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
| [GetPageCount](./getpagecount/) | Obtiene el recuento total de páginas del workbook. |
| [GetPageSizeInch](./getpagesizeinch/) | Obtenga el tamaño de página en pulgadas de la imagen de salida. |
| [ToImage](./toimage/) | Renderiza todo el workbook como Imagen Tiff a stream. |
| [ToImage_String](./toimage_string/) | Renderiza todo el workbook como Imagen Tiff a un archivo. |
| [ToImage_Int_String](./toimage_int_string/) | Renderiza una página determinada a un archivo. |
| [ToImage_Int](./toimage_int/) | Renderiza una página determinada a un stream. |
| [Dispose](./dispose/) | Libera los recursos creados y utilizados para el renderizado. |
