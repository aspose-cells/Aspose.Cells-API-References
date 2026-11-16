---
title: "ProtectedRange-Klasse"
linktitle: "ProtectedRange"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "ProtectedRange-Klasse. Kapselt das Objekt, das den protectedrange in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/protectedrange/
---

## ProtectedRange class

Ein angegebener Bereich, der bearbeitet werden darf, wenn der Blattschutz aktiviert ist.

```go

type ProtectedRange struct  {
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
| [GetName](./getname/) | Liefert den Titel des Bereichs. Dieser wird als Bezeichner verwendet, nicht als Definition eines benannten Bereichs. |
| [SetName](./setname/) | Liefert den Titel des Bereichs. Dieser wird als Bezeichner verwendet, nicht als Definition eines benannten Bereichs. |
| [GetCellArea](./getcellarea/) | Liefert das CellArea-Objekt, das den zu schützenden Zellbereich darstellt. |
| [GetAreas](./getareas/) | Liefert alle referenzierten Bereiche. |
| [AddArea](./addarea/) | Fügt diesem einen referenzierten Bereich hinzu |
| [IsProtectedWithPassword](./isprotectedwithpassword/) | Gibt an, ob das Arbeitsblatt mit einem Passwort geschützt ist. |
| [GetPassword](./getpassword/) | Stellt das Passwort zum Schutz des Bereichs dar. |
| [SetPassword](./setpassword/) | Stellt das Passwort zum Schutz des Bereichs dar. |
| [GetSecurityDescriptor](./getsecuritydescriptor/) | Der Sicherheitsdeskriptor definiert Benutzerkonten, die diesen Bereich bearbeiten dürfen, ohne ein Passwort anzugeben, um auf den Bereich zuzugreifen. |
| [SetSecurityDescriptor](./setsecuritydescriptor/) | Der Sicherheitsdeskriptor definiert Benutzerkonten, die diesen Bereich bearbeiten dürfen, ohne ein Passwort anzugeben, um auf den Bereich zuzugreifen. |
