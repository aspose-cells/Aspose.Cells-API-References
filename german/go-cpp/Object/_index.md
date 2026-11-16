---
title: "Objektklasse."
linktitle: "Objekt."
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "Objektklasse. Kapselt das Objekt, das ein Objekt in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/object/
---

## Object class

Objektklasse.

```go

type Object struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewObject](./newobject/) | Standardkonstruktor. Erstellt ein leeres Objekt. |
| [NewObject_Bool](./newobject_bool/) | Konstruiert aus einem bool-Wert. |
| [NewObject_Integer8](./newobject_integer8/) | Konstruiert aus einem int8_t-Wert. |
| [NewObject_Byte](./newobject_byte/) | Konstruiert aus einem uint8_t-Wert. |
| [NewObject_Int16](./newobject_int16/) | Konstruiert aus einem int16_t-Wert. |
| [NewObject_UInteger16](./newobject_uinteger16/) | Konstruiert aus einem uint16_t-Wert. |
| [NewObject_Int](./newobject_int/) | Konstruiert aus einem int32_t-Wert. |
| [NewObject_UInteger](./newobject_uinteger/) | Konstruiert aus einem uint32_t-Wert. |
| [NewObject_Int64](./newobject_int64/) | Konstruiert aus einem int64_t-Wert. |
| [NewObject_ULong](./newobject_ulong/) | Konstruiert aus einem uint64_t-Wert. |
| [NewObject_Float](./newobject_float/) | Konstruiert aus einem float-Wert. |
| [NewObject_Double](./newobject_double/) | Konstruiert aus einem double-Wert. |
| [NewObject_Date](./newobject_date/) | Konstruiert aus einem Date-Wert. |
| [NewObject_Color](./newobject_color/) | Konstruiert aus einem Color-Wert. |
| [NewObject_String](./newobject_string/) | Konstruiert aus einem U16String-Wert. |
| [NewObject_Range](./newobject_range/) | Konstruiert aus einem Range-Wert. |
| [NewObject_ObjectArray](./newobject_objectarray/) | Konstruiert aus einem eindimensionalen Array. |
| [NewObject_Object2Array](./newobject_object2array/) | Konstruiert aus einem zweidimensionalen Array. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [GetType](./gettype/) | Ermittelt den ObjectType des Objekts. |
| [GetNumberType](./getnumbertype/) | Ermittelt den NumberType des Objekts. |
| [IsBool](./isbool/) | Prüft, ob das Objekt ein bool-Wert ist. |
| [IsNumber](./isnumber/) | Prüft, ob das Objekt ein Zahlenwert ist. |
| [IsInt32](./isint32/) | Prüft, ob das Objekt ein int32_t-Wert ist. |
| [IsDouble](./isdouble/) | Prüft, ob das Objekt ein double-Wert ist. |
| [IsNull](./isnull/) | Prüft, ob das Objekt null ist. |
| [IsDate](./isdate/) | Prüft, ob das Objekt ein Date-Wert ist. |
| [IsColor](./iscolor/) | Prüft, ob das Objekt ein Color-Wert ist. |
| [IsString](./isstring/) | Prüft, ob das Objekt ein String-Wert ist. |
| [IsRange](./isrange/) | Prüft, ob das Objekt ein Range-Zeiger ist. |
| [IsReferredArea](./isreferredarea/) | Prüft, ob das Objekt ein ReferredArea-Zeiger ist. |
| [IsArray1D](./isarray1d/) | Prüft, ob das Objekt ein eindimensionales Array ist. |
| [IsArray2D](./isarray2d/) | Prüft, ob das Objekt ein zweidimensionales Array ist. |
| [IsObject](./isobject/) | Prüft, ob das Objekt ein Objektzeiger ist. |
| [ToBool](./tobool/) | Ermittelt den bool-Wert. |
| [ToInt8](./toint8/) | Ermittelt den int8_t-Wert. |
| [ToUInt8](./touint8/) | Ermittelt den uint8_t-Wert. |
| [ToInt16](./toint16/) | Ermittelt den int16_t-Wert. |
| [ToUInt16](./touint16/) | Ermittelt den uint16_t-Wert. |
| [ToInt32](./toint32/) | Ermittelt den int32_t-Wert. |
| [ToUInt32](./touint32/) | Ruft den uint32_t-Wert ab. |
| [ToInt64](./toint64/) | Ruft den int64_t-Wert ab. |
| [ToUInt64](./touint64/) | Ruft den uint64_t-Wert ab. |
| [ToFloat](./tofloat/) | Ruft den float-Wert ab. |
| [ToDouble](./todouble/) | Ruft den double-Wert ab. |
| [AsInt32](./asint32/) | Konvertiert das Objekt in einen int32_t-Wert, wenn das Objekt vom Zahlentyp ist. |
| [AsDouble](./asdouble/) | Konvertiert das Objekt in einen double-Wert, wenn das Objekt vom Zahlentyp ist. |
| [ToString](./tostring/) | Ruft den String-Wert ab. |
| [ToDate](./todate/) | Ruft den Date-Wert ab. |
| [ToColor](./tocolor/) | Ruft den Color-Wert ab. |
| [ToRange](./torange/) | Ruft den Range-Wert ab. |
| [ToReferredArea](./toreferredarea/) | Ruft den ReferredArea-Wert ab. |
| [ToArray1D](./toarray1d/) | Ruft den ein-dimensionalen Array-Wert ab. |
| [ToArray2D](./toarray2d/) | Ruft den zwei-dimensionalen Array-Wert ab. |
