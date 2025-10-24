##Object Class
'Object class. Encapsulates the object that represents object in Go.'
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
|[NewObject](./newobject/) | Default constructor. Constructs an empty object. |
|[NewObject_Bool](./newobject_bool/) | Constructs from a bool value. |
|[NewObject_Integer8](./newobject_integer8/) | Constructs from an int8_t value. |
|[NewObject_Byte](./newobject_byte/) | Constructs from an uint8_t value. |
|[NewObject_Int16](./newobject_int16/) | Constructs from an int16_t value. |
|[NewObject_UInteger16](./newobject_uinteger16/) | Constructs from an uint16_t value. |
|[NewObject_Int](./newobject_int/) | Constructs from an int32_t value. |
|[NewObject_UInteger](./newobject_uinteger/) | Constructs from an uint32_t value. |
|[NewObject_Int64](./newobject_int64/) | Constructs from an int64_t value. |
|[NewObject_ULong](./newobject_ulong/) | Constructs from an uint64_t value. |
|[NewObject_Float](./newobject_float/) | Constructs from a float value. |
|[NewObject_Double](./newobject_double/) | Constructs from a double value. |
|[NewObject_Date](./newobject_date/) | Constructs from a Date value. |
|[NewObject_Color](./newobject_color/) | Constructs from a Color value. |
|[NewObject_String](./newobject_string/) | Constructs from U16String value. |
|[NewObject_Range](./newobject_range/) | Constructs from a Range value. |
|[NewObject_ObjectArray](./newobject_objectarray/) | Constructs from a one-dimensional array. |
|[NewObject_Object2Array](./newobject_object2array/) | Constructs from a two-dimensional array. |
## Methods
| Method | Description |
| --- | --- |
|[GetType](./gettype/) | Gets the ObjectType of the object. |
|[GetNumberType](./getnumbertype/) | Gets the NumberType of the object. |
|[IsBool](./isbool/) | Checks whether the object is a bool value. |
|[IsNumber](./isnumber/) | Checks whether the object is a number value. |
|[IsInt32](./isint32/) | Checks whether the object is an int32_t value. |
|[IsDouble](./isdouble/) | Checks whether the object is a double value. |
|[IsNull](./isnull/) | Checks whether the object is null. |
|[IsDate](./isdate/) | Checks whether the object is a Date value. |
|[IsColor](./iscolor/) | Checks whether the object is a Color value. |
|[IsString](./isstring/) | Checks whether the object is a String value. |
|[IsRange](./isrange/) | Checks whether the object is a Range pointer. |
|[IsReferredArea](./isreferredarea/) | Checks whether the object is a ReferredArea pointer. |
|[IsArray1D](./isarray1d/) | Checks whether the object is a one-dimensional array. |
|[IsArray2D](./isarray2d/) | Checks whether the object is a two-dimensional array. |
|[IsObject](./isobject/) | Checks whether the object is an object pointer. |
|[ToBool](./tobool/) | Gets the bool value. |
|[ToInt8](./toint8/) | Gets the int8_t value. |
|[ToUInt8](./touint8/) | Gets the uint8_t value. |
|[ToInt16](./toint16/) | Gets the int16_t value. |
|[ToUInt16](./touint16/) | Gets the uint16_t value. |
|[ToInt32](./toint32/) | Gets the int32_t value. |
|[ToUInt32](./touint32/) | Gets the uint32_t value. |
|[ToInt64](./toint64/) | Gets the int64_t value. |
|[ToUInt64](./touint64/) | Gets the uint64_t value. |
|[ToFloat](./tofloat/) | Gets the float value. |
|[ToDouble](./todouble/) | Gets the double value. |
|[AsInt32](./asint32/) | Converts the object to an int32_t value, if object is number type. |
|[AsDouble](./asdouble/) | Converts the object to a double value, if object is number type. |
|[ToString](./tostring/) | Gets the String value. |
|[ToDate](./todate/) | Gets the Date value. |
|[ToColor](./tocolor/) | Gets the Color value. |
|[ToRange](./torange/) | Gets the Range value. |
|[ToReferredArea](./toreferredarea/) | Gets the ReferredArea value. |
|[ToArray1D](./toarray1d/) | Gets the one-dimensional array value. |
|[ToArray2D](./toarray2d/) | Gets the two-dimensional array value. |
