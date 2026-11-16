---
title: "IconSet Klasse"
linktitle: "IconSet"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "IconSet Klasse. Kapselt das Objekt, das iconset in Go repräsentiert."
type: docs
weight: 200
url: /de/go-cpp/iconset/
---

## IconSet class

Beschreibt die IconSet-Bedingte-Formatierungsregel. Diese bedingte Formatierungsregel wendet Symbole auf Zellen entsprechend ihrer Werte an.

```go

type IconSet struct  {
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
| [GetCfIcons](./getcficons/) | Lese theConditionalFormattingIcon aus der Sammlung |
| [GetCfvos](./getcfvos/) | Rufen Sie die CFValueObjects-Instanz ab. |
| [GetType](./gettype/) | Abrufen oder Festlegen des Anzeigetypus des Symbolsatzes. Das Festlegen des Typs prüft automatisch, ob die aktuelle Anzahl der Cfods mit dem neuen Typ übereinstimmt. Wenn nicht, werden alte Cfods bereinigt und Standard‑Cfods hinzugefügt. |
| [SetType](./settype/) | Abrufen oder Festlegen des Anzeigetypus des Symbolsatzes. Das Festlegen des Typs prüft automatisch, ob die aktuelle Anzahl der Cfods mit dem neuen Typ übereinstimmt. Wenn nicht, werden alte Cfods bereinigt und Standard‑Cfods hinzugefügt. |
| [IsCustom](./iscustom/) | Gibt an, ob der Symbolsatz benutzerdefiniert ist. Standardwert ist false. |
| [GetShowValue](./getshowvalue/) | Abrufen oder Festlegen des Flags, das angibt, ob die Werte der Zellen angezeigt werden sollen, auf die dieser Symbolsatz angewendet wird. Standardwert ist true. |
| [SetShowValue](./setshowvalue/) | Abrufen oder Festlegen des Flags, das angibt, ob die Werte der Zellen angezeigt werden sollen, auf die dieser Symbolsatz angewendet wird. Standardwert ist true. |
| [GetReverse](./getreverse/) | Abrufen oder Festlegen des Flags, das angibt, ob die Standardreihenfolge der Symbole in diesem Symbolsatz umgekehrt wird. Standardwert ist false. |
| [SetReverse](./setreverse/) | Abrufen oder Festlegen des Flags, das angibt, ob die Standardreihenfolge der Symbole in diesem Symbolsatz umgekehrt wird. Standardwert ist false. |
