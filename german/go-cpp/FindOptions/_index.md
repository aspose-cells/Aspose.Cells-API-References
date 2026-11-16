---
title: "FindOptions Klasse"
linktitle: "FindOptions"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "FindOptions Klasse. Kapselt das Objekt, das FindOptions in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/findoptions/
---

## FindOptions class

Stellt Suchoptionen dar.

```go

type FindOptions struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewFindOptions](./newfindoptions/) | Standardkonstruktor. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetCaseSensitive](./getcasesensitive/) | Gibt an, ob die gesuchte Zeichenkette Groß-/Kleinschreibung beachtet. |
| [SetCaseSensitive](./setcasesensitive/) | Gibt an, ob die gesuchte Zeichenkette Groß-/Kleinschreibung beachtet. |
| [GetLookAtType](./getlookattype/) | Typ prüfen. |
| [SetLookAtType](./setlookattype/) | Typ prüfen. |
| [GetRange](./getrange/) | Liest und setzt den gesuchten Bereich. |
| [SetRange](./setrange/) | Setzt den gesuchten Bereich. |
| [IsRangeSet](./israngeset/) | Gibt an, ob der gesuchte Bereich festgelegt ist. |
| [GetSearchBackward](./getsearchbackward/) | Ob rückwärts nach Zellen gesucht wird. |
| [SetSearchBackward](./setsearchbackward/) | Ob rückwärts nach Zellen gesucht wird. |
| [GetSearchOrderByRows](./getsearchorderbyrows/) | Gibt an, ob die Suchreihenfolge nach Zeilen oder Spalten erfolgt. |
| [SetSearchOrderByRows](./setsearchorderbyrows/) | Gibt an, ob die Suchreihenfolge nach Zeilen oder Spalten erfolgt. |
| [GetLookInType](./getlookintype/) | Im Typ suchen. |
| [SetLookInType](./setlookintype/) | Im Typ suchen. |
| [GetRegexKey](./getregexkey/) | Gibt an, ob der gesuchte Schlüssel ein Regex ist. Wenn true, wird der gesuchte Schlüssel als Regex behandelt und geparst. Andernfalls wird der Schlüssel gemäß den Regeln in MS Excel geparst. |
| [SetRegexKey](./setregexkey/) | Gibt an, ob der gesuchte Schlüssel ein Regex ist. Wenn true, wird der gesuchte Schlüssel als Regex behandelt und geparst. Andernfalls wird der Schlüssel gemäß den Regeln in MS Excel geparst. |
| [GetValueTypeSensitive](./getvaluetypesensitive/) | Gibt an, ob der Typ des gesuchten Zellwerts mit dem gesuchten Schlüssel übereinstimmen soll. |
| [SetValueTypeSensitive](./setvaluetypesensitive/) | Gibt an, ob der Typ des gesuchten Zellwerts mit dem gesuchten Schlüssel übereinstimmen soll. |
| [GetStyle](./getstyle/) | Das Format, nach dem gesucht werden soll. |
| [SetStyle](./setstyle/) | Das Format, nach dem gesucht werden soll. |
| [GetConvertNumericData](./getconvertnumericdata/) | Liest oder setzt einen Wert, der angibt, ob der gesuchte Zeichenkettenwert in numerische Daten konvertiert wird. |
| [SetConvertNumericData](./setconvertnumericdata/) | Liest oder setzt einen Wert, der angibt, ob der gesuchte Zeichenkettenwert in numerische Daten konvertiert wird. |
