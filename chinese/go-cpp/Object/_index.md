---
title: "对象类"
linktitle: "对象"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "对象类。封装在 Go 中表示对象的对象。"
type: docs
weight: 200
url: /zh/go-cpp/object/
---

## Object class

对象类。

```go

type Object struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewObject](./newobject/) | 默认构造函数。构造一个空对象。 |
| [NewObject_Bool](./newobject_bool/) | 从布尔值构造。 |
| [NewObject_Integer8](./newobject_integer8/) | 从 int8_t 值构造。 |
| [NewObject_Byte](./newobject_byte/) | 从 uint8_t 值构造。 |
| [NewObject_Int16](./newobject_int16/) | 从 int16_t 值构造。 |
| [NewObject_UInteger16](./newobject_uinteger16/) | 从 uint16_t 值构造。 |
| [NewObject_Int](./newobject_int/) | 从 int32_t 值构造。 |
| [NewObject_UInteger](./newobject_uinteger/) | 从 uint32_t 值构造。 |
| [NewObject_Int64](./newobject_int64/) | 从 int64_t 值构造。 |
| [NewObject_ULong](./newobject_ulong/) | 从 uint64_t 值构造。 |
| [NewObject_Float](./newobject_float/) | 从 float 值构造。 |
| [NewObject_Double](./newobject_double/) | 从 double 值构造。 |
| [NewObject_Date](./newobject_date/) | 从 Date 值构造。 |
| [NewObject_Color](./newobject_color/) | 从 Color 值构造。 |
| [NewObject_String](./newobject_string/) | 从 U16String 值构造。 |
| [NewObject_Range](./newobject_range/) | 从 Range 值构造。 |
| [NewObject_ObjectArray](./newobject_objectarray/) | 从一维数组构造。 |
| [NewObject_Object2Array](./newobject_object2array/) | 从二维数组构造。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [GetType](./gettype/) | 获取对象的 ObjectType。 |
| [GetNumberType](./getnumbertype/) | 获取对象的 NumberType。 |
| [IsBool](./isbool/) | 检查对象是否为 bool 值。 |
| [IsNumber](./isnumber/) | 检查对象是否为 number 值。 |
| [IsInt32](./isint32/) | 检查对象是否为 int32_t 值。 |
| [IsDouble](./isdouble/) | 检查对象是否为 double 值。 |
| [IsNull](./isnull/) | 检查对象是否为 null。 |
| [IsDate](./isdate/) | 检查对象是否为 Date 值。 |
| [IsColor](./iscolor/) | 检查对象是否为 Color 值。 |
| [IsString](./isstring/) | 检查对象是否为 String 值。 |
| [IsRange](./isrange/) | 检查对象是否为 Range 指针。 |
| [IsReferredArea](./isreferredarea/) | 检查对象是否为 ReferredArea 指针。 |
| [IsArray1D](./isarray1d/) | 检查对象是否为一维数组。 |
| [IsArray2D](./isarray2d/) | 检查对象是否为二维数组。 |
| [IsObject](./isobject/) | 检查对象是否为对象指针。 |
| [ToBool](./tobool/) | 获取 bool 值。 |
| [ToInt8](./toint8/) | 获取 int8_t 值。 |
| [ToUInt8](./touint8/) | 获取 uint8_t 值。 |
| [ToInt16](./toint16/) | 获取 int16_t 值。 |
| [ToUInt16](./touint16/) | 获取 uint16_t 值。 |
| [ToInt32](./toint32/) | 获取 int32_t 值。 |
| [ToUInt32](./touint32/) | 获取 uint32_t 值。 |
| [ToInt64](./toint64/) | 获取 int64_t 值。 |
| [ToUInt64](./touint64/) | 获取 uint64_t 值。 |
| [ToFloat](./tofloat/) | 获取 float 值。 |
| [ToDouble](./todouble/) | 获取 double 值。 |
| [AsInt32](./asint32/) | 如果对象为数值类型，则将对象转换为 int32_t 值。 |
| [AsDouble](./asdouble/) | 如果对象为数值类型，则将对象转换为 double 值。 |
| [ToString](./tostring/) | 获取 String 值。 |
| [ToDate](./todate/) | 获取 Date 值。 |
| [ToColor](./tocolor/) | 获取 Color 值。 |
| [ToRange](./torange/) | 获取 Range 值。 |
| [ToReferredArea](./toreferredarea/) | 获取 ReferredArea 值。 |
| [ToArray1D](./toarray1d/) | 获取一维数组值。 |
| [ToArray2D](./toarray2d/) | 获取二维数组值。 |
