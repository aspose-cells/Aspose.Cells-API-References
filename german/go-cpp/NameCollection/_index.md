---
title: "NameCollection Klasse"
linktitle: "NameCollection"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "NameCollection Klasse. Kapselt das Objekt, das namecollection in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/namecollection/
---

## NameCollection class

Stellt eine Sammlung aller <see cref=\"Name\"/>-Objekte im Tabellenblatt dar.

```go

type NameCollection struct  {
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
| [Add](./add/) | Definiert einen neuen Namen. |
| [Get_Int](./get_int/) | Liefert das Name-Element am angegebenen Index. |
| [Filter](./filter/) | Ruft alle definierten Namen nach Geltungsbereich ab. |
| [Get_String](./get_string/) | Ruft das Name-Element mit dem angegebenen Namen ab. |
| [Remove_stringArray](./remove_stringarray/) | Entfernt ein Array von Namen |
| [Remove_String](./remove_string/) | Entfernt den Namen. |
| [RemoveAt](./removeat/) | Entfernt den Namen am angegebenen Index. |
| [Clear](./clear/) | Entfernt alle definierten Namen, die nicht von Formeln und Datenquellen referenziert werden. Wenn der definierte Name referenziert wird, setzen wir nur Name.ReferTo auf null und blenden ihn aus. |
| [RemoveDuplicateNames](./removeduplicatenames/) | Entfernt die doppelten definierten Namen |
| [Sort](./sort/) | Sortiert definierte Namen. |
| [GetCount](./getcount/) | Liefert die Anzahl der im Objekt enthaltenen Elemente. |
