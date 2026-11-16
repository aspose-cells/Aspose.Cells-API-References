---
title: "Classe d'objet"
linktitle: "Objet"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe d'objet. Encapsule l'objet qui représente l'objet en Go."
type: docs
weight: 200
url: /fr/go-cpp/object/
---

## Object class

Classe d'objet.

```go

type Object struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewObject](./newobject/) | Constructeur par défaut. Construit un objet vide. |
| [NewObject_Bool](./newobject_bool/) | Construit à partir d'une valeur booléenne. |
| [NewObject_Integer8](./newobject_integer8/) | Construit à partir d'une valeur int8_t. |
| [NewObject_Byte](./newobject_byte/) | Construit à partir d'une valeur uint8_t. |
| [NewObject_Int16](./newobject_int16/) | Construit à partir d'une valeur int16_t. |
| [NewObject_UInteger16](./newobject_uinteger16/) | Construit à partir d'une valeur uint16_t. |
| [NewObject_Int](./newobject_int/) | Construit à partir d'une valeur int32_t. |
| [NewObject_UInteger](./newobject_uinteger/) | Construit à partir d'une valeur uint32_t. |
| [NewObject_Int64](./newobject_int64/) | Construit à partir d'une valeur int64_t. |
| [NewObject_ULong](./newobject_ulong/) | Construit à partir d'une valeur uint64_t. |
| [NewObject_Float](./newobject_float/) | Construit à partir d'une valeur float. |
| [NewObject_Double](./newobject_double/) | Construit à partir d'une valeur double. |
| [NewObject_Date](./newobject_date/) | Construit à partir d'une valeur Date. |
| [NewObject_Color](./newobject_color/) | Construit à partir d'une valeur Color. |
| [NewObject_String](./newobject_string/) | Construit à partir d'une valeur U16String. |
| [NewObject_Range](./newobject_range/) | Construit à partir d'une valeur Range. |
| [NewObject_ObjectArray](./newobject_objectarray/) | Construit à partir d'un tableau unidimensionnel. |
| [NewObject_Object2Array](./newobject_object2array/) | Construit à partir d'un tableau bidimensionnel. |

## Méthodes

| Méthode | Description |
| --- | --- |
| [GetType](./gettype/) | Obtient le ObjectType de l'objet. |
| [GetNumberType](./getnumbertype/) | Obtient le NumberType de l'objet. |
| [IsBool](./isbool/) | Vérifie si l'objet est une valeur bool. |
| [IsNumber](./isnumber/) | Vérifie si l'objet est une valeur numérique. |
| [IsInt32](./isint32/) | Vérifie si l'objet est une valeur int32_t. |
| [IsDouble](./isdouble/) | Vérifie si l'objet est une valeur double. |
| [IsNull](./isnull/) | Vérifie si l'objet est nul. |
| [IsDate](./isdate/) | Vérifie si l'objet est une valeur Date. |
| [IsColor](./iscolor/) | Vérifie si l'objet est une valeur Color. |
| [IsString](./isstring/) | Vérifie si l'objet est une valeur String. |
| [IsRange](./isrange/) | Vérifie si l'objet est un pointeur Range. |
| [IsReferredArea](./isreferredarea/) | Vérifie si l'objet est un pointeur ReferredArea. |
| [IsArray1D](./isarray1d/) | Vérifie si l'objet est un tableau unidimensionnel. |
| [IsArray2D](./isarray2d/) | Vérifie si l'objet est un tableau bidimensionnel. |
| [IsObject](./isobject/) | Vérifie si l'objet est un pointeur d'objet. |
| [ToBool](./tobool/) | Obtient la valeur booléenne. |
| [ToInt8](./toint8/) | Obtient la valeur int8_t. |
| [ToUInt8](./touint8/) | Obtient la valeur uint8_t. |
| [ToInt16](./toint16/) | Obtient la valeur int16_t. |
| [ToUInt16](./touint16/) | Obtient la valeur uint16_t. |
| [ToInt32](./toint32/) | Obtient la valeur int32_t. |
| [ToUInt32](./touint32/) | Obtient la valeur uint32_t. |
| [ToInt64](./toint64/) | Obtient la valeur int64_t. |
| [ToUInt64](./touint64/) | Obtient la valeur uint64_t. |
| [ToFloat](./tofloat/) | Obtient la valeur float. |
| [ToDouble](./todouble/) | Obtient la valeur double. |
| [AsInt32](./asint32/) | Convertit l'objet en une valeur int32_t, si l'objet est de type numérique. |
| [AsDouble](./asdouble/) | Convertit l'objet en une valeur double, si l'objet est de type numérique. |
| [ToString](./tostring/) | Obtient la valeur String. |
| [ToDate](./todate/) | Obtient la valeur Date. |
| [ToColor](./tocolor/) | Obtient la valeur Color. |
| [ToRange](./torange/) | Obtient la valeur Range. |
| [ToReferredArea](./toreferredarea/) | Obtient la valeur ReferredArea. |
| [ToArray1D](./toarray1d/) | Obtient la valeur du tableau unidimensionnel. |
| [ToArray2D](./toarray2d/) | Obtient la valeur du tableau bidimensionnel. |
