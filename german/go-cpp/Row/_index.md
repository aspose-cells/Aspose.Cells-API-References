---
title: "Zeilenklasse"
linktitle: "Zeile"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "Zeilenklasse. Kapselt das Objekt, das eine Zeile in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/row/
---

## Row class

Stellt eine einzelne Zeile in einem Arbeitsblatt dar.

```go

type Row struct  {
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
| [GetCellByIndex](./getcellbyindex/) | Hole die Zelle anhand eines bestimmten Indexes in der Zellsammlung dieser Zeile. |
| [IsBlank](./isblank/) | Gibt an, ob die Zeile Daten enthält |
| [Get](./get/) | Liefert die Zelle. |
| [GetEnumerator](./getenumerator/) | Liefert den Zellen-Enumerator |
| [GetEnumerator_Bool_Bool](./getenumerator_bool_bool/) | Liefert einen Enumerator, der die Zellen dieser Zeile durchläuft. |
| [GetCellOrNull](./getcellornull/) | Liefert die Zelle oder null am angegebenen Index. |
| [IsCollapsed](./iscollapsed/) | ob die Zeile zusammengeklappt ist |
| [SetIsCollapsed](./setiscollapsed/) | ob die Zeile zusammengeklappt ist |
| [GetHeight](./getheight/) | Liefert und setzt die Zeilenhöhe in Punkten. |
| [SetHeight](./setheight/) | Liefert und setzt die Zeilenhöhe in Punkten. |
| [IsHidden](./ishidden/) | Gibt an, ob die Zeile ausgeblendet ist. |
| [SetIsHidden](./setishidden/) | Gibt an, ob die Zeile ausgeblendet ist. |
| [GetIndex](./getindex/) | Liefert den Index dieser Zeile. |
| [GetGroupLevel](./getgrouplevel/) | Liefert die Gruppenebene der Zeile. |
| [SetGroupLevel](./setgrouplevel/) | Liefert die Gruppenebene der Zeile. |
| [IsHeightMatched](./isheightmatched/) | Gibt an, ob die Zeilenhöhe mit der aktuellen Standardschriftart-Einstellung der Arbeitsmappe übereinstimmt. Der Wert True dieser Eigenschaft bedeutet außerdem, dass die Zeilenhöhe "automatisch" ist, ohne dass der Benutzer einen benutzerdefinierten Höhenwert festgelegt hat. |
| [SetIsHeightMatched](./setisheightmatched/) | Gibt an, ob die Zeilenhöhe mit der aktuellen Standardschriftart-Einstellung der Arbeitsmappe übereinstimmt. Der Wert True dieser Eigenschaft bedeutet außerdem, dass die Zeilenhöhe "automatisch" ist, ohne dass der Benutzer einen benutzerdefinierten Höhenwert festgelegt hat. |
| [GetStyle](./getstyle/) | Liefert den Stil dieser Zeile. |
| [SetStyle](./setstyle/) | Setzt den Stil dieser Zeile. |
| [GetHasCustomStyle](./gethascustomstyle/) | Gibt an, ob diese Zeile benutzerdefinierte Stileinstellungen hat (anders als der Standard, der von der Arbeitsmappe geerbt wird). |
| [CopySettings](./copysettings/) | Kopiere die Einstellungen der Zeile, wie Stil, Höhe, Sichtbarkeit, ...usw. |
| [GetFirstCell](./getfirstcell/) | Liefert das erste Zellenobjekt in der Zeile. |
| [GetFirstDataCell](./getfirstdatacell/) | Liefert die erste nicht-leere Zelle in der Zeile. |
| [GetLastCell](./getlastcell/) | Liefert das letzte Zellenobjekt in der Zeile. |
| [GetLastDataCell](./getlastdatacell/) | Liefert die letzte nicht-leere Zelle in der Zeile. |
| [ApplyStyle](./applystyle/) | Wendet Formate für eine gesamte Zeile an. |
| [Equals_Object](./equals_object/) | Prüft, ob dieses Objekt auf dieselbe Zeile wie ein anderes verweist. |
| [Equals_Row](./equals_row/) | Prüft, ob dieses Objekt auf dieselbe Zeile wie ein anderes Zeilenobjekt verweist. |
