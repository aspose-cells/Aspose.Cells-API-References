---
title: "فئة الكائن"
linktitle: "الكائن"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة الكائن. تغلف الكائن الذي يمثل الكائن في Go."
type: docs
weight: 200
url: /ar/go-cpp/object/
---

## Object class

فئة الكائن.

```go

type Object struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewObject](./newobject/) | منشئ افتراضي. ينشئ كائنًا فارغًا. |
| [NewObject_Bool](./newobject_bool/) | ينشئ من قيمة منطقية. |
| [NewObject_Integer8](./newobject_integer8/) | ينشئ من قيمة int8_t. |
| [NewObject_Byte](./newobject_byte/) | ينشئ من قيمة uint8_t. |
| [NewObject_Int16](./newobject_int16/) | ينشئ من قيمة int16_t. |
| [NewObject_UInteger16](./newobject_uinteger16/) | يُنشئ من قيمة uint16_t. |
| [NewObject_Int](./newobject_int/) | يُنشئ من قيمة int32_t. |
| [NewObject_UInteger](./newobject_uinteger/) | يُنشئ من قيمة uint32_t. |
| [NewObject_Int64](./newobject_int64/) | يُنشئ من قيمة int64_t. |
| [NewObject_ULong](./newobject_ulong/) | يُنشئ من قيمة uint64_t. |
| [NewObject_Float](./newobject_float/) | يُنشئ من قيمة float. |
| [NewObject_Double](./newobject_double/) | يُنشئ من قيمة double. |
| [NewObject_Date](./newobject_date/) | يُنشئ من قيمة Date. |
| [NewObject_Color](./newobject_color/) | يُنشئ من قيمة Color. |
| [NewObject_String](./newobject_string/) | يُنشئ من قيمة U16String. |
| [NewObject_Range](./newobject_range/) | يُنشئ من قيمة Range. |
| [NewObject_ObjectArray](./newobject_objectarray/) | يُنشئ من مصفوفة أحادية البُعد. |
| [NewObject_Object2Array](./newobject_object2array/) | يُنشئ من مصفوفة ثنائية البُعد. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [GetType](./gettype/) | يحصل على ObjectType للكائن. |
| [GetNumberType](./getnumbertype/) | يحصل على NumberType للكائن. |
| [IsBool](./isbool/) | يتحقق مما إذا كان الكائن قيمة bool. |
| [IsNumber](./isnumber/) | يتحقق مما إذا كان الكائن قيمة عددية. |
| [IsInt32](./isint32/) | يتحقق مما إذا كان الكائن قيمة int32_t. |
| [IsDouble](./isdouble/) | يتحقق مما إذا كان الكائن قيمة double. |
| [IsNull](./isnull/) | يتحقق مما إذا كان الكائن null. |
| [IsDate](./isdate/) | يتحقق مما إذا كان الكائن قيمة Date. |
| [IsColor](./iscolor/) | يتحقق مما إذا كان الكائن قيمة Color. |
| [IsString](./isstring/) | يتحقق مما إذا كان الكائن قيمة String. |
| [IsRange](./isrange/) | يتحقق مما إذا كان الكائن مؤشر Range. |
| [IsReferredArea](./isreferredarea/) | يتحقق مما إذا كان الكائن مؤشر ReferredArea. |
| [IsArray1D](./isarray1d/) | يتحقق مما إذا كان الكائن مصفوفة أحادية البعد. |
| [IsArray2D](./isarray2d/) | يتحقق مما إذا كان الكائن مصفوفة ثنائية البعد. |
| [IsObject](./isobject/) | يتحقق مما إذا كان الكائن مؤشرًا لكائن. |
| [ToBool](./tobool/) | يحصل على قيمة bool. |
| [ToInt8](./toint8/) | يحصل على قيمة int8_t. |
| [ToUInt8](./touint8/) | يحصل على قيمة uint8_t. |
| [ToInt16](./toint16/) | يحصل على قيمة int16_t. |
| [ToUInt16](./touint16/) | يحصل على قيمة uint16_t. |
| [ToInt32](./toint32/) | يحصل على قيمة int32_t. |
| [ToUInt32](./touint32/) | يحصل على قيمة uint32_t. |
| [ToInt64](./toint64/) | يحصل على قيمة int64_t. |
| [ToUInt64](./touint64/) | يحصل على قيمة uint64_t. |
| [ToFloat](./tofloat/) | يحصل على قيمة float. |
| [ToDouble](./todouble/) | يحصل على قيمة double. |
| [AsInt32](./asint32/) | يحوّل الكائن إلى قيمة int32_t إذا كان الكائن من نوع عدد. |
| [AsDouble](./asdouble/) | يحوّل الكائن إلى قيمة double إذا كان الكائن من نوع عدد. |
| [ToString](./tostring/) | يحصل على قيمة String. |
| [ToDate](./todate/) | يحصل على قيمة Date. |
| [ToColor](./tocolor/) | يحصل على قيمة Color. |
| [ToRange](./torange/) | يحصل على قيمة Range. |
| [ToReferredArea](./toreferredarea/) | يحصل على قيمة ReferredArea. |
| [ToArray1D](./toarray1d/) | يحصل على قيمة مصفوفة أحادية البعد. |
| [ToArray2D](./toarray2d/) | يحصل على قيمة مصفوفة ثنائية البعد. |
