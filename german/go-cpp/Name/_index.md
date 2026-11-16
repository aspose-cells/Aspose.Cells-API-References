---
title: "Name Klasse"
linktitle: "Name"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "Name Klasse. Kapselt das Objekt, das name in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/name/
---

## Name class

Stellt einen definierten Namen für einen Zellbereich dar.

```go

type Name struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetComment](./getcomment/) | Liest und setzt den Kommentar des Namens. Gilt nur für Excel 2007 oder höhere Versionen. |
| [SetComment](./setcomment/) | Liest und setzt den Kommentar des Namens. Gilt nur für Excel 2007 oder höhere Versionen. |
| [GetText](./gettext/) | Liest den Namens‑Text des Objekts. |
| [SetText](./settext/) | Liest den Namens‑Text des Objekts. |
| [GetFullText](./getfulltext/) | Liest den vollständigen Namenstext des Objekts mit der Geltungsbereichseinstellung. |
| [GetRefersTo](./getrefersto/) | Gibt die Formel zurück oder setzt sie, auf die der Name verweist, beginnend mit einem Gleichheitszeichen. |
| [SetRefersTo_String](./setrefersto_string/) | Gibt die Formel zurück oder setzt sie, auf die der Name verweist, beginnend mit einem Gleichheitszeichen. |
| [GetR1C1RefersTo](./getr1c1refersto/) | Liest oder setzt eine R1C1‑Referenz des Namens. |
| [SetR1C1RefersTo](./setr1c1refersto/) | Liest oder setzt eine R1C1‑Referenz des Namens. |
| [GetRefersTo_Bool_Bool](./getrefersto_bool_bool/) | Lese die Referenz dieses Namens. |
| [GetRefersTo_Bool_Bool_Int_Int](./getrefersto_bool_bool_int_int/) | Lese die Referenz dieses Namens basierend auf der angegebenen Zelle. |
| [SetRefersTo_String_Bool_Bool](./setrefersto_string_bool_bool/) | Setze die Referenz dieses Namens. |
| [IsReferred](./isreferred/) | Gibt an, ob dieser Name von anderen Formeln referenziert wird. |
| [IsVisible](./isvisible/) | Gibt an, ob der Name sichtbar ist. |
| [SetIsVisible](./setisvisible/) | Gibt an, ob der Name sichtbar ist. |
| [GetSheetIndex](./getsheetindex/) | Gibt an, ob dieser Name zu Arbeitsmappe oder Arbeitsblatt gehört. 0 = Globaler Name, sonst Index zum Blatt (einsbasiert) |
| [SetSheetIndex](./setsheetindex/) | Gibt an, ob dieser Name zu Arbeitsmappe oder Arbeitsblatt gehört. 0 = Globaler Name, sonst Index zum Blatt (einsbasiert) |
| [ToString](./tostring/) | Gibt einen String zurück, der das aktuelle Range‑Objekt darstellt. |
| [GetRanges](./getranges/) | Liest alle Bereiche, die von diesem Namen referenziert werden. |
| [GetRanges_Bool](./getranges_bool/) | Liest alle Bereiche, die von diesem Namen referenziert werden. |
| [GetReferredAreas](./getreferredareas/) | Ermittelt alle Referenzen, die von diesem Namen referenziert werden. |
| [GetRange](./getrange/) | Ermittelt den Bereich, wenn dieser Name auf einen Bereich verweist. |
| [GetRange_Bool](./getrange_bool/) | Ermittelt den Bereich, wenn dieser Name auf einen Bereich verweist |
| [GetRange_Int_Int_Int](./getrange_int_int_int/) | Ermittelt den Bereich, wenn dieser Name auf einen Bereich verweist. Wenn die Referenz dieses Namens nicht absolut ist, kann der Bereich für verschiedene Zellen unterschiedlich sein. |
