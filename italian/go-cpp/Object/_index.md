---
title: "Classe Oggetto"
linktitle: "Oggetto"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe oggetto. Incapsula l'oggetto che rappresenta l'oggetto in Go."
type: docs
weight: 200
url: /it/go-cpp/object/
---

## Object class

Classe oggetto.

```go

type Object struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewObject](./newobject/) | Costruttore predefinito. Costruisce un oggetto vuoto. |
| [NewObject_Bool](./newobject_bool/) | Costruisce da un valore booleano. |
| [NewObject_Integer8](./newobject_integer8/) | Costruisce da un valore int8_t. |
| [NewObject_Byte](./newobject_byte/) | Costruisce da un valore uint8_t. |
| [NewObject_Int16](./newobject_int16/) | Costruisce da un valore int16_t. |
| [NewObject_UInteger16](./newobject_uinteger16/) | Costruisce da un valore uint16_t. |
| [NewObject_Int](./newobject_int/) | Costruisce da un valore int32_t. |
| [NewObject_UInteger](./newobject_uinteger/) | Costruisce da un valore uint32_t. |
| [NewObject_Int64](./newobject_int64/) | Costruisce da un valore int64_t. |
| [NewObject_ULong](./newobject_ulong/) | Costruisce da un valore uint64_t. |
| [NewObject_Float](./newobject_float/) | Costruisce da un valore float. |
| [NewObject_Double](./newobject_double/) | Costruisce da un valore double. |
| [NewObject_Date](./newobject_date/) | Costruisce da un valore Date. |
| [NewObject_Color](./newobject_color/) | Costruisce da un valore Color. |
| [NewObject_String](./newobject_string/) | Costruisce da un valore U16String. |
| [NewObject_Range](./newobject_range/) | Costruisce da un valore Range. |
| [NewObject_ObjectArray](./newobject_objectarray/) | Costruisce da un array monodimensionale. |
| [NewObject_Object2Array](./newobject_object2array/) | Costruisce da un array bidimensionale. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [GetType](./gettype/) | Ottiene l'ObjectType dell'oggetto. |
| [GetNumberType](./getnumbertype/) | Ottiene il NumberType dell'oggetto. |
| [IsBool](./isbool/) | Verifica se l'oggetto è un valore bool. |
| [IsNumber](./isnumber/) | Verifica se l'oggetto è un valore numerico. |
| [IsInt32](./isint32/) | Verifica se l'oggetto è un valore int32_t. |
| [IsDouble](./isdouble/) | Verifica se l'oggetto è un valore double. |
| [IsNull](./isnull/) | Verifica se l'oggetto è nullo. |
| [IsDate](./isdate/) | Verifica se l'oggetto è un valore Date. |
| [IsColor](./iscolor/) | Verifica se l'oggetto è un valore Color. |
| [IsString](./isstring/) | Verifica se l'oggetto è un valore String. |
| [IsRange](./isrange/) | Verifica se l'oggetto è un puntatore Range. |
| [IsReferredArea](./isreferredarea/) | Verifica se l'oggetto è un puntatore ReferredArea. |
| [IsArray1D](./isarray1d/) | Verifica se l'oggetto è un array monodimensionale. |
| [IsArray2D](./isarray2d/) | Verifica se l'oggetto è un array bidimensionale. |
| [IsObject](./isobject/) | Verifica se l'oggetto è un puntatore a oggetto. |
| [ToBool](./tobool/) | Ottiene il valore bool. |
| [ToInt8](./toint8/) | Ottiene il valore int8_t. |
| [ToUInt8](./touint8/) | Ottiene il valore uint8_t. |
| [ToInt16](./toint16/) | Ottiene il valore int16_t. |
| [ToUInt16](./touint16/) | Ottiene il valore uint16_t. |
| [ToInt32](./toint32/) | Ottiene il valore int32_t. |
| [ToUInt32](./touint32/) | Ottiene il valore uint32_t. |
| [ToInt64](./toint64/) | Ottiene il valore int64_t. |
| [ToUInt64](./touint64/) | Ottiene il valore uint64_t. |
| [ToFloat](./tofloat/) | Ottiene il valore float. |
| [ToDouble](./todouble/) | Ottiene il valore double. |
| [AsInt32](./asint32/) | Converte l'oggetto in un valore int32_t, se l'oggetto è di tipo numerico. |
| [AsDouble](./asdouble/) | Converte l'oggetto in un valore double, se l'oggetto è di tipo numerico. |
| [ToString](./tostring/) | Ottiene il valore String. |
| [ToDate](./todate/) | Ottiene il valore Date. |
| [ToColor](./tocolor/) | Ottiene il valore Color. |
| [ToRange](./torange/) | Ottiene il valore Range. |
| [ToReferredArea](./toreferredarea/) | Ottiene il valore ReferredArea. |
| [ToArray1D](./toarray1d/) | Ottiene il valore dell'array monodimensionale. |
| [ToArray2D](./toarray2d/) | Ottiene il valore dell'array bidimensionale. |
