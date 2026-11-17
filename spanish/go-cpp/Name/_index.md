---
title: "Name Clase"
linktitle: "Name"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "Name clase. Encapsula el objeto que representa name en Go."
type: docs
weight: 200
url: /es/go-cpp/name/
---

## Name class

Represents a defined name for a range of cells.

```go

type Name struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |

## Methods

| Method | Description |
| --- | --- |
| [IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
| [GetComment](./getcomment/) | Obtiene y establece el comentario del nombre.Solo se aplica a Excel 2007 o versiones superiores. |
| [SetComment](./setcomment/) | Obtiene y establece el comentario del nombre.Solo se aplica a Excel 2007 o versiones superiores. |
| [GetText](./gettext/) | Obtiene el texto del nombre del objeto. |
| [SetText](./settext/) | Obtiene el texto del nombre del objeto. |
| [GetFullText](./getfulltext/) | Obtiene el texto completo del nombre del objeto con la configuración de alcance. |
| [GetRefersTo](./getrefersto/) | Devuelve o establece la fórmula a la que el nombre está definido para referirse, comenzando con un signo igual. |
| [SetRefersTo_String](./setrefersto_string/) | Devuelve o establece la fórmula a la que el nombre está definido para referirse, comenzando con un signo igual. |
| [GetR1C1RefersTo](./getr1c1refersto/) | Obtiene o establece una referencia R1C1 del Nombre. |
| [SetR1C1RefersTo](./setr1c1refersto/) | Obtiene o establece una referencia R1C1 del Nombre. |
| [GetRefersTo_Bool_Bool](./getrefersto_bool_bool/) | Obtenga la referencia de este Nombre. |
| [GetRefersTo_Bool_Bool_Int_Int](./getrefersto_bool_bool_int_int/) | Obtenga la referencia de este Nombre basada en la celda especificada. |
| [SetRefersTo_String_Bool_Bool](./setrefersto_string_bool_bool/) | Establezca la referencia de este Nombre. |
| [IsReferred](./isreferred/) | Indica si este nombre es referenciado por otras fórmulas. |
| [IsVisible](./isvisible/) | Indica si el nombre es visible. |
| [SetIsVisible](./setisvisible/) | Indica si el nombre es visible. |
| [GetSheetIndex](./getsheetindex/) | Indica a qué pertenece este nombre: Libro de trabajo o Hoja de cálculo. 0 = Nombre global, de lo contrario índice a la hoja (basado en 1). |
| [SetSheetIndex](./setsheetindex/) | Indica a qué pertenece este nombre: Libro de trabajo o Hoja de cálculo. 0 = Nombre global, de lo contrario índice a la hoja (basado en 1). |
| [ToString](./tostring/) | Returns a string represents the current Range object. |
| [GetRanges](./getranges/) | Obtiene todos los rangos referidos por este nombre. |
| [GetRanges_Bool](./getranges_bool/) | Obtiene todos los rangos referidos por este nombre. |
| [GetReferredAreas](./getreferredareas/) | Obtiene todas las referencias referidas por este nombre. |
| [GetRange](./getrange/) | Obtiene el rango si este nombre se refiere a un rango. |
| [GetRange_Bool](./getrange_bool/) | Obtiene el rango si este nombre se refiere a un rango |
| [GetRange_Int_Int_Int](./getrange_int_int_int/) | Obtiene el rango si este nombre se refiere a un rango. Si la referencia de este nombre no es absoluta, el rango puede ser diferente para distintas celdas. |
