---
title: "CustomDocumentPropertyCollection Klasse"
linktitle: "CustomDocumentPropertyCollection"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "CustomDocumentPropertyCollection Klasse. Kapselt das Objekt, das customdocumentpropertycollection in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/customdocumentpropertycollection/
---

## CustomDocumentPropertyCollection class

Eine Sammlung benutzerdefinierter Dokumenteigenschaften.

```go

type CustomDocumentPropertyCollection struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewCustomDocumentPropertyCollection](./newcustomdocumentpropertycollection/) | Konstruiert aus einem übergeordneten Objekt. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [Add_String_String](./add_string_string/) | Erstellt eine neue benutzerdefinierte Dokumenteigenschaft des Datentyps <b>PropertyType.String</b>. |
| [Add_String_Int](./add_string_int/) | Erstellt eine neue benutzerdefinierte Dokumenteigenschaft des Datentyps <b>PropertyType.Number</b>. |
| [Add_String_Date](./add_string_date/) | Erstellt eine neue benutzerdefinierte Dokumenteigenschaft des Datentyps <b>PropertyType.DateTime</b>. |
| [Add_String_Bool](./add_string_bool/) | Erstellt eine neue benutzerdefinierte Dokumenteigenschaft des Datentyps <b>PropertyType.Boolean</b>. |
| [Add_String_Double](./add_string_double/) | Erstellt eine neue benutzerdefinierte Dokumenteigenschaft des Datentyps <b>PropertyType.Float</b>. |
| [AddLinkToContent](./addlinktocontent/) | Erstellt eine neue benutzerdefinierte Dokumenteigenschaft, die mit Inhalt verknüpft ist. |
| [UpdateLinkedPropertyValue](./updatelinkedpropertyvalue/) | Aktualisiert die Werte aller benutzerdefinierten Eigenschaften, die mit Inhalt verknüpft sind (usecell-Wert des verknüpften Bereichs, um den Wert der benutzerdefinierten Eigenschaft zu aktualisieren). |
| [UpdateLinkedRange](./updatelinkedrange/) | Aktualisiert alle Bereiche, die mit benutzerdefinierten Eigenschaften verknüpft sind (verwende den Wert dercustom document property, um den Zellenwert des verknüpften Bereichs zu aktualisieren). |
| [Get_Int](./get_int/) | Gibt ein DocumentProperty-Objekt nach Index zurück. |
| [Contains](./contains/) | Gibt true zurück, wenn eine Eigenschaft mit dem angegebenen Namen in der Sammlung existiert. |
| [IndexOf](./indexof/) | Ermittelt den Index einer Eigenschaft nach Namen. |
| [Remove](./remove/) | Entfernt eine Eigenschaft mit dem angegebenen Namen aus der Sammlung. |
| [RemoveAt](./removeat/) | Entfernt eine Eigenschaft am angegebenen Index. |
| [GetCount](./getcount/) | Liefert die Anzahl der im Objekt enthaltenen Elemente. |
