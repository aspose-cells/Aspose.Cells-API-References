---
title: "Класс объекта"
linktitle: "Объект"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс объекта. Инкапсулирует объект, который представляет объект в Go."
type: docs
weight: 200
url: /ru/go-cpp/object/
---

## Object class

Класс объекта.

```go

type Object struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewObject](./newobject/) | Конструктор по умолчанию. Создает пустой объект. |
| [NewObject_Bool](./newobject_bool/) | Создает из логического значения. |
| [NewObject_Integer8](./newobject_integer8/) | Создает из значения int8_t. |
| [NewObject_Byte](./newobject_byte/) | Создает из значения uint8_t. |
| [NewObject_Int16](./newobject_int16/) | Создает из значения int16_t. |
| [NewObject_UInteger16](./newobject_uinteger16/) | Создаёт из значения uint16_t. |
| [NewObject_Int](./newobject_int/) | Создаёт из значения int32_t. |
| [NewObject_UInteger](./newobject_uinteger/) | Создаёт из значения uint32_t. |
| [NewObject_Int64](./newobject_int64/) | Создаёт из значения int64_t. |
| [NewObject_ULong](./newobject_ulong/) | Создаёт из значения uint64_t. |
| [NewObject_Float](./newobject_float/) | Создаёт из значения float. |
| [NewObject_Double](./newobject_double/) | Создаёт из значения double. |
| [NewObject_Date](./newobject_date/) | Создаёт из значения Date. |
| [NewObject_Color](./newobject_color/) | Создаёт из значения Color. |
| [NewObject_String](./newobject_string/) | Создаёт из значения U16String. |
| [NewObject_Range](./newobject_range/) | Создаёт из значения Range. |
| [NewObject_ObjectArray](./newobject_objectarray/) | Создаёт из одномерного массива. |
| [NewObject_Object2Array](./newobject_object2array/) | Создаёт из двумерного массива. |

## Методы

| Метод | Описание |
| --- | --- |
| [GetType](./gettype/) | Получает ObjectType объекта. |
| [GetNumberType](./getnumbertype/) | Получает NumberType объекта. |
| [IsBool](./isbool/) | Проверяет, является ли объект значением bool. |
| [IsNumber](./isnumber/) | Проверяет, является ли объект числовым значением. |
| [IsInt32](./isint32/) | Проверяет, является ли объект значением int32_t. |
| [IsDouble](./isdouble/) | Проверяет, является ли объект значением double. |
| [IsNull](./isnull/) | Проверяет, является ли объект null. |
| [IsDate](./isdate/) | Проверяет, является ли объект значением Date. |
| [IsColor](./iscolor/) | Проверяет, является ли объект значением Color. |
| [IsString](./isstring/) | Проверяет, является ли объект значением String. |
| [IsRange](./isrange/) | Проверяет, является ли объект указателем Range. |
| [IsReferredArea](./isreferredarea/) | Проверяет, является ли объект указателем ReferredArea. |
| [IsArray1D](./isarray1d/) | Проверяет, является ли объект одномерным массивом. |
| [IsArray2D](./isarray2d/) | Проверяет, является ли объект двумерным массивом. |
| [IsObject](./isobject/) | Проверяет, является ли объект указателем на объект. |
| [ToBool](./tobool/) | Получает значение типа bool. |
| [ToInt8](./toint8/) | Получает значение типа int8_t. |
| [ToUInt8](./touint8/) | Получает значение типа uint8_t. |
| [ToInt16](./toint16/) | Получает значение типа int16_t. |
| [ToUInt16](./touint16/) | Получает значение типа uint16_t. |
| [ToInt32](./toint32/) | Получает значение типа int32_t. |
| [ToUInt32](./touint32/) | Получает значение типа uint32_t. |
| [ToInt64](./toint64/) | Получает значение типа int64_t. |
| [ToUInt64](./touint64/) | Получает значение типа uint64_t. |
| [ToFloat](./tofloat/) | Получает значение типа float. |
| [ToDouble](./todouble/) | Получает значение типа double. |
| [AsInt32](./asint32/) | Преобразует объект в значение типа int32_t, если объект является числовым типом. |
| [AsDouble](./asdouble/) | Преобразует объект в значение типа double, если объект является числовым типом. |
| [ToString](./tostring/) | Получает значение типа String. |
| [ToDate](./todate/) | Получает значение типа Date. |
| [ToColor](./tocolor/) | Получает значение типа Color. |
| [ToRange](./torange/) | Получает значение типа Range. |
| [ToReferredArea](./toreferredarea/) | Получает значение типа ReferredArea. |
| [ToArray1D](./toarray1d/) | Получает значение одномерного массива. |
| [ToArray2D](./toarray2d/) | Получает значение двумерного массива. |
