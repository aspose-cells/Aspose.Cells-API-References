---
title: "CopyOptions Klasse"
linktitle: "CopyOptions"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "CopyOptions Klasse. Kapselt das Objekt, das copyoptions in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/copyoptions/
---

## CopyOptions class

Stellt die Kopieroptionen dar.

```go

type CopyOptions struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewCopyOptions](./newcopyoptions/) | CopyOptions Konstruktor. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetKeepMacros](./getkeepmacros/) | Gibt an, ob Makros beibehalten werden; |
| [SetKeepMacros](./setkeepmacros/) | Gibt an, ob Makros beibehalten werden; |
| [GetExtendToAdjacentRange](./getextendtoadjacentrange/) | Gibt an, ob Bereiche beim Kopieren des Bereichs in den angrenzenden Bereich erweitert werden. |
| [SetExtendToAdjacentRange](./setextendtoadjacentrange/) | Gibt an, ob Bereiche beim Kopieren des Bereichs in den angrenzenden Bereich erweitert werden. |
| [GetCopyNames](./getcopynames/) | Gibt an, ob die Namen kopiert werden. |
| [SetCopyNames](./setcopynames/) | Gibt an, ob die Namen kopiert werden. |
| [GetCopyInvalidFormulasAsValues](./getcopyinvalidformulasasvalues/) | Wenn die Formel für das Ziel nicht gültig ist, nur Werte kopieren. |
| [SetCopyInvalidFormulasAsValues](./setcopyinvalidformulasasvalues/) | Wenn die Formel für das Ziel nicht gültig ist, nur Werte kopieren. |
| [GetColumnCharacterWidth](./getcolumncharacterwidth/) | Gibt an, ob die Spaltenbreite in Zeichen kopiert wird. |
| [SetColumnCharacterWidth](./setcolumncharacterwidth/) | Gibt an, ob die Spaltenbreite in Zeichen kopiert wird. |
| [GetReferToSheetWithSameName](./getrefertosheetwithsamename/) | In MS Excel, wenn Formeln, die sich auf andere Arbeitsblätter beziehen, beim Kopieren eines Arbeitsblatts in ein anderes kopiert werden, sollten die kopierten Formeln auf die Quellarbeitsmappe verweisen. Allerdings kann der Benutzer in manchen Situationen benötigen, dass die kopierten Formeln auf Arbeitsblätter mit demselben Namen in derselben Arbeitsmappe verweisen, zum Beispiel wenn diese Arbeitsblätter bereits vor diesem Kopiervorgang kopiert wurden, dann sollte diese Eigenschaft auf true gesetzt werden. |
| [SetReferToSheetWithSameName](./setrefertosheetwithsamename/) | In MS Excel, wenn Formeln, die sich auf andere Arbeitsblätter beziehen, beim Kopieren eines Arbeitsblatts in ein anderes kopiert werden, sollten die kopierten Formeln auf die Quellarbeitsmappe verweisen. Allerdings kann der Benutzer in manchen Situationen benötigen, dass die kopierten Formeln auf Arbeitsblätter mit demselben Namen in derselben Arbeitsmappe verweisen, zum Beispiel wenn diese Arbeitsblätter bereits vor diesem Kopiervorgang kopiert wurden, dann sollte diese Eigenschaft auf true gesetzt werden. |
| [GetReferToDestinationSheet](./getrefertodestinationsheet/) | Beim Kopieren des Bereichs in derselben Datei und wenn das Diagramm auf das Quellblatt verweist, bedeutet False, dass die Datenquelle des kopierten Diagramms nicht geändert wird. True bedeutet, dass die Datenquelle des kopierten Diagramms auf das Zielblatt verweist. |
| [SetReferToDestinationSheet](./setrefertodestinationsheet/) | Beim Kopieren des Bereichs in derselben Datei und wenn das Diagramm auf das Quellblatt verweist, bedeutet False, dass die Datenquelle des kopierten Diagramms nicht geändert wird. True bedeutet, dass die Datenquelle des kopierten Diagramms auf das Zielblatt verweist. |
| [GetUpdateInvalidReferencesToTargetSheet](./getupdateinvalidreferencestotargetsheet/) | Gibt an, ob auf das Zielarbeitsblatt verwiesen werden soll, wenn das referenzierte Arbeitsblatt nicht kopiert wird. |
| [SetUpdateInvalidReferencesToTargetSheet](./setupdateinvalidreferencestotargetsheet/) | Gibt an, ob auf das Zielarbeitsblatt verwiesen werden soll, wenn das referenzierte Arbeitsblatt nicht kopiert wird. |
