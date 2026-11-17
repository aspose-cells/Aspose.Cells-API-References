---
title: "Clase de objeto"
linktitle: "Objeto"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "Clase de objeto. Encapsula el objeto que representa al objeto en Go."
type: docs
weight: 200
url: /es/go-cpp/object/
---

## Object class

Object class.

```go

type Object struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |
| [NewObject](./newobject/) | Constructor predeterminado. Construye un objeto vacío. |
| [NewObject_Bool](./newobject_bool/) | Construye a partir de un valor bool. |
| [NewObject_Integer8](./newobject_integer8/) | Construye a partir de un valor int8_t. |
| [NewObject_Byte](./newobject_byte/) | Construye a partir de un valor uint8_t. |
| [NewObject_Int16](./newobject_int16/) | Construye a partir de un valor int16_t. |
| [NewObject_UInteger16](./newobject_uinteger16/) | Construye a partir de un valor uint16_t. |
| [NewObject_Int](./newobject_int/) | Construye a partir de un valor int32_t. |
| [NewObject_UInteger](./newobject_uinteger/) | Construye a partir de un valor uint32_t. |
| [NewObject_Int64](./newobject_int64/) | Construye a partir de un valor int64_t. |
| [NewObject_ULong](./newobject_ulong/) | Construye a partir de un valor uint64_t. |
| [NewObject_Float](./newobject_float/) | Construye a partir de un valor float. |
| [NewObject_Double](./newobject_double/) | Construye a partir de un valor double. |
| [NewObject_Date](./newobject_date/) | Construye a partir de un valor Date. |
| [NewObject_Color](./newobject_color/) | Construye a partir de un valor Color. |
| [NewObject_String](./newobject_string/) | Construye a partir de un valor U16String. |
| [NewObject_Range](./newobject_range/) | Construye a partir de un valor Range. |
| [NewObject_ObjectArray](./newobject_objectarray/) | Construye a partir de una matriz unidimensional. |
| [NewObject_Object2Array](./newobject_object2array/) | Construye a partir de una matriz bidimensional. |

## Methods

| Method | Description |
| --- | --- |
| [GetType](./gettype/) | Obtiene el ObjectType del objeto. |
| [GetNumberType](./getnumbertype/) | Obtiene el NumberType del objeto. |
| [IsBool](./isbool/) | Comprueba si el objeto es un valor bool. |
| [IsNumber](./isnumber/) | Comprueba si el objeto es un valor numérico. |
| [IsInt32](./isint32/) | Comprueba si el objeto es un valor int32_t. |
| [IsDouble](./isdouble/) | Comprueba si el objeto es un valor double. |
| [IsNull](./isnull/) | Comprueba si el objeto es nulo. |
| [IsDate](./isdate/) | Comprueba si el objeto es un valor Date. |
| [IsColor](./iscolor/) | Comprueba si el objeto es un valor Color. |
| [IsString](./isstring/) | Comprueba si el objeto es un valor String. |
| [IsRange](./isrange/) | Comprueba si el objeto es un puntero Range. |
| [IsReferredArea](./isreferredarea/) | Comprueba si el objeto es un puntero ReferredArea. |
| [IsArray1D](./isarray1d/) | Comprueba si el objeto es una matriz unidimensional. |
| [IsArray2D](./isarray2d/) | Comprueba si el objeto es una matriz bidimensional. |
| [IsObject](./isobject/) | Comprueba si el objeto es un puntero a objeto. |
| [ToBool](./tobool/) | Obtiene el valor bool. |
| [ToInt8](./toint8/) | Obtiene el valor int8_t. |
| [ToUInt8](./touint8/) | Obtiene el valor uint8_t. |
| [ToInt16](./toint16/) | Obtiene el valor int16_t. |
| [ToUInt16](./touint16/) | Obtiene el valor uint16_t. |
| [ToInt32](./toint32/) | Obtiene el valor int32_t. |
| [ToUInt32](./touint32/) | Obtiene el valor uint32_t. |
| [ToInt64](./toint64/) | Obtiene el valor int64_t. |
| [ToUInt64](./touint64/) | Obtiene el valor uint64_t. |
| [ToFloat](./tofloat/) | Obtiene el valor float. |
| [ToDouble](./todouble/) | Obtiene el valor double. |
| [AsInt32](./asint32/) | Convierte el objeto a un valor int32_t, si el objeto es de tipo numérico. |
| [AsDouble](./asdouble/) | Convierte el objeto a un valor double, si el objeto es de tipo numérico. |
| [ToString](./tostring/) | Obtiene el valor String. |
| [ToDate](./todate/) | Obtiene el valor Date. |
| [ToColor](./tocolor/) | Obtiene el valor Color. |
| [ToRange](./torange/) | Obtiene el valor Range. |
| [ToReferredArea](./toreferredarea/) | Obtiene el valor ReferredArea. |
| [ToArray1D](./toarray1d/) | Obtiene el valor de la matriz unidimensional. |
| [ToArray2D](./toarray2d/) | Obtiene el valor de la matriz bidimensional. |
