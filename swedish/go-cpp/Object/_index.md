---
title: "Objektklass"
linktitle: "Objekt"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "Objektklass. Inkapslar objektet som representerar objekt i Go."
type: docs
weight: 200
url: /sv/go-cpp/object/
---

## Object class

Objektklass.

```go

type Object struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewObject](./newobject/) | Standardkonstruktor. Skapar ett tomt objekt. |
| [NewObject_Bool](./newobject_bool/) | Skapar från ett booleskt värde. |
| [NewObject_Integer8](./newobject_integer8/) | Skapar från ett int8_t‑värde. |
| [NewObject_Byte](./newobject_byte/) | Skapar från ett uint8_t‑värde. |
| [NewObject_Int16](./newobject_int16/) | Skapar från ett int16_t‑värde. |
| [NewObject_UInteger16](./newobject_uinteger16/) | Skapar från ett uint16_t‑värde. |
| [NewObject_Int](./newobject_int/) | Skapar från ett int32_t‑värde. |
| [NewObject_UInteger](./newobject_uinteger/) | Skapar från ett uint32_t‑värde. |
| [NewObject_Int64](./newobject_int64/) | Skapar från ett int64_t‑värde. |
| [NewObject_ULong](./newobject_ulong/) | Skapar från ett uint64_t‑värde. |
| [NewObject_Float](./newobject_float/) | Skapar från ett float‑värde. |
| [NewObject_Double](./newobject_double/) | Skapar från ett double‑värde. |
| [NewObject_Date](./newobject_date/) | Skapar från ett Date‑värde. |
| [NewObject_Color](./newobject_color/) | Skapar från ett Color‑värde. |
| [NewObject_String](./newobject_string/) | Skapar från U16String‑värde. |
| [NewObject_Range](./newobject_range/) | Skapar från ett Range‑värde. |
| [NewObject_ObjectArray](./newobject_objectarray/) | Skapar från en endimensionell array. |
| [NewObject_Object2Array](./newobject_object2array/) | Skapar från en tvådimensionell array. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [GetType](./gettype/) | Hämtar ObjectType för objektet. |
| [GetNumberType](./getnumbertype/) | Hämtar NumberType för objektet. |
| [IsBool](./isbool/) | Kontrollerar om objektet är ett booleskt värde. |
| [IsNumber](./isnumber/) | Kontrollerar om objektet är ett numeriskt värde. |
| [IsInt32](./isint32/) | Kontrollerar om objektet är ett int32_t‑värde. |
| [IsDouble](./isdouble/) | Kontrollerar om objektet är ett double‑värde. |
| [IsNull](./isnull/) | Kontrollerar om objektet är null. |
| [IsDate](./isdate/) | Kontrollerar om objektet är ett Date‑värde. |
| [IsColor](./iscolor/) | Kontrollerar om objektet är ett Color‑värde. |
| [IsString](./isstring/) | Kontrollerar om objektet är ett String‑värde. |
| [IsRange](./isrange/) | Kontrollerar om objektet är en Range‑pekare. |
| [IsReferredArea](./isreferredarea/) | Kontrollerar om objektet är en ReferredArea‑pekare. |
| [IsArray1D](./isarray1d/) | Kontrollerar om objektet är en endimensionell array. |
| [IsArray2D](./isarray2d/) | Kontrollerar om objektet är en tvådimensionell array. |
| [IsObject](./isobject/) | Kontrollerar om objektet är en objektpekare. |
| [ToBool](./tobool/) | Hämtar det booleska värdet. |
| [ToInt8](./toint8/) | Hämtar int8_t‑värdet. |
| [ToUInt8](./touint8/) | Hämtar uint8_t‑värdet. |
| [ToInt16](./toint16/) | Hämtar int16_t‑värdet. |
| [ToUInt16](./touint16/) | Hämtar uint16_t‑värdet. |
| [ToInt32](./toint32/) | Hämtar int32_t‑värdet. |
| [ToUInt32](./touint32/) | Hämtar uint32_t‑värdet. |
| [ToInt64](./toint64/) | Hämtar int64_t‑värdet. |
| [ToUInt64](./touint64/) | Hämtar uint64_t‑värdet. |
| [ToFloat](./tofloat/) | Hämtar float‑värdet. |
| [ToDouble](./todouble/) | Hämtar double‑värdet. |
| [AsInt32](./asint32/) | Konverterar objektet till ett int32_t‑värde, om objektet är av numerisk typ. |
| [AsDouble](./asdouble/) | Konverterar objektet till ett double‑värde om objektet är av numerisk typ. |
| [ToString](./tostring/) | Hämtar String‑värdet. |
| [ToDate](./todate/) | Hämtar Date‑värdet. |
| [ToColor](./tocolor/) | Hämtar Color‑värdet. |
| [ToRange](./torange/) | Hämtar Range‑värdet. |
| [ToReferredArea](./toreferredarea/) | Hämtar ReferredArea‑värdet. |
| [ToArray1D](./toarray1d/) | Hämtar värdet för en endimensionell array. |
| [ToArray2D](./toarray2d/) | Hämtar värdet för en tvådimensionell array. |
