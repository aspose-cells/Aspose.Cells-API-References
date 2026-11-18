---
title: "Nesne Sınıfı"
linktitle: "Nesne"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "Nesne sınıfı. Go dilinde nesneyi temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/object/
---

## Object class

Nesne sınıfı.

```go

type Object struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewObject](./newobject/) | Varsayılan yapıcı. Boş bir nesne oluşturur. |
| [NewObject_Bool](./newobject_bool/) | Bir bool değerinden oluşturur. |
| [NewObject_Integer8](./newobject_integer8/) | Bir int8_t değerinden oluşturur. |
| [NewObject_Byte](./newobject_byte/) | Bir uint8_t değerinden oluşturur. |
| [NewObject_Int16](./newobject_int16/) | Bir int16_t değerinden oluşturur. |
| [NewObject_UInteger16](./newobject_uinteger16/) | uint16_t değerinden oluşturur. |
| [NewObject_Int](./newobject_int/) | int32_t değerinden oluşturur. |
| [NewObject_UInteger](./newobject_uinteger/) | uint32_t değerinden oluşturur. |
| [NewObject_Int64](./newobject_int64/) | int64_t değerinden oluşturur. |
| [NewObject_ULong](./newobject_ulong/) | uint64_t değerinden oluşturur. |
| [NewObject_Float](./newobject_float/) | float değerinden oluşturur. |
| [NewObject_Double](./newobject_double/) | double değerinden oluşturur. |
| [NewObject_Date](./newobject_date/) | Date değerinden oluşturur. |
| [NewObject_Color](./newobject_color/) | Color değerinden oluşturur. |
| [NewObject_String](./newobject_string/) | U16String değerinden oluşturur. |
| [NewObject_Range](./newobject_range/) | Range değerinden oluşturur. |
| [NewObject_ObjectArray](./newobject_objectarray/) | tek boyutlu bir diziden oluşturur. |
| [NewObject_Object2Array](./newobject_object2array/) | iki boyutlu bir diziden oluşturur. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [GetType](./gettype/) | Nesnenin ObjectType değerini alır. |
| [GetNumberType](./getnumbertype/) | Nesnenin NumberType değerini alır. |
| [IsBool](./isbool/) | Nesnenin bool değeri olup olmadığını denetler. |
| [IsNumber](./isnumber/) | Nesnenin sayı değeri olup olmadığını denetler. |
| [IsInt32](./isint32/) | Nesnenin int32_t değeri olup olmadığını denetler. |
| [IsDouble](./isdouble/) | Nesnenin double değeri olup olmadığını denetler. |
| [IsNull](./isnull/) | Nesnenin null olup olmadığını denetler. |
| [IsDate](./isdate/) | Nesnenin Date değeri olup olmadığını denetler. |
| [IsColor](./iscolor/) | Nesnenin Color değeri olup olmadığını denetler. |
| [IsString](./isstring/) | Nesnenin String değeri olup olmadığını denetler. |
| [IsRange](./isrange/) | Nesnenin Range işaretçisi olup olmadığını denetler. |
| [IsReferredArea](./isreferredarea/) | Nesnenin ReferredArea işaretçisi olup olmadığını denetler. |
| [IsArray1D](./isarray1d/) | Nesnenin tek boyutlu bir dizi olup olmadığını denetler. |
| [IsArray2D](./isarray2d/) | Nesnenin iki boyutlu bir dizi olup olmadığını denetler. |
| [IsObject](./isobject/) | Nesnenin bir nesne işaretçisi olup olmadığını denetler. |
| [ToBool](./tobool/) | bool değerini alır. |
| [ToInt8](./toint8/) | int8_t değerini alır. |
| [ToUInt8](./touint8/) | uint8_t değerini alır. |
| [ToInt16](./toint16/) | int16_t değerini alır. |
| [ToUInt16](./touint16/) | uint16_t değerini alır. |
| [ToInt32](./toint32/) | int32_t değerini alır. |
| [ToUInt32](./touint32/) | uint32_t değerini alır. |
| [ToInt64](./toint64/) | int64_t değerini alır. |
| [ToUInt64](./touint64/) | uint64_t değerini alır. |
| [ToFloat](./tofloat/) | float değerini alır. |
| [ToDouble](./todouble/) | double değerini alır. |
| [AsInt32](./asint32/) | Nesneyi int32_t değerine dönüştürür, eğer nesne sayı tipindeyse. |
| [AsDouble](./asdouble/) | Nesneyi double değerine dönüştürür, eğer nesne sayı tipindeyse. |
| [ToString](./tostring/) | String değerini alır. |
| [ToDate](./todate/) | Date değerini alır. |
| [ToColor](./tocolor/) | Color değerini alır. |
| [ToRange](./torange/) | Range değerini alır. |
| [ToReferredArea](./toreferredarea/) | ReferredArea değerini alır. |
| [ToArray1D](./toarray1d/) | tek boyutlu dizi değerini alır. |
| [ToArray2D](./toarray2d/) | iki boyutlu dizi değerini alır. |
