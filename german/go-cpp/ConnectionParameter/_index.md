---
title: "ConnectionParameter Klasse"
linktitle: "ConnectionParameter"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "ConnectionParameter Klasse. Kapselt das Objekt, das connectionparameter in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/connectionparameter/
---

## ConnectionParameter class

Gibt Eigenschaften zu allen Parametern an, die mit externen Datenverbindungen verwendet werden. Parameter sind für ODBC‑ und Webabfragen gültig.

```go

type ConnectionParameter struct  {
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
| [GetSqlType](./getsqltype/) | SQL-Datentyp des Parameters. Nur gültig für ODBC-Quellen. |
| [SetSqlType](./setsqltype/) | SQL-Datentyp des Parameters. Nur gültig für ODBC-Quellen. |
| [GetRefreshOnChange](./getrefreshonchange/) | Flag, das angibt, ob die Abfrage automatisch aktualisiert werden soll, wenn sich der Inhalt einer Zelle, die den Parameterwert bereitstellt, ändert. Wenn wahr, werden externe Daten bei jeder Änderung mit dem neuen Parameterwert aktualisiert. Wenn falsch, werden externe Daten nur aktualisiert, wenn der Benutzer dies anfordert oder ein anderes Ereignis die Aktualisierung auslöst (z. B. beim Öffnen der Arbeitsmappe). |
| [SetRefreshOnChange](./setrefreshonchange/) | Flag, das angibt, ob die Abfrage automatisch aktualisiert werden soll, wenn sich der Inhalt einer Zelle, die den Parameterwert bereitstellt, ändert. Wenn wahr, werden externe Daten bei jeder Änderung mit dem neuen Parameterwert aktualisiert. Wenn falsch, werden externe Daten nur aktualisiert, wenn der Benutzer dies anfordert oder ein anderes Ereignis die Aktualisierung auslöst (z. B. beim Öffnen der Arbeitsmappe). |
| [GetPrompt](./getprompt/) | Eingabeaufforderungszeichenfolge für den Parameter. Wird dem Tabellenbenutzer zusammen mit einer Eingabe‑UI angezeigt, um den Parameterwert vor dem Aktualisieren der externen Daten zu erfassen. Wird nur verwendet, wenn parameterType = prompt. |
| [SetPrompt](./setprompt/) | Eingabeaufforderungszeichenfolge für den Parameter. Wird dem Tabellenbenutzer zusammen mit einer Eingabe‑UI angezeigt, um den Parameterwert vor dem Aktualisieren der externen Daten zu erfassen. Wird nur verwendet, wenn parameterType = prompt. |
| [GetType](./gettype/) | Verwendeter Parametertyp. Wenn parameterType = value, wird der Wert aus boolean, double, integer oder string verwendet. In diesem Fall wird erwartet, dass nur einer von {boolean, double, integer, or string} angegeben wird. |
| [SetType](./settype/) | Verwendeter Parametertyp. Wenn parameterType = value, wird der Wert aus boolean, double, integer oder string verwendet. In diesem Fall wird erwartet, dass nur einer von {boolean, double, integer, or string} angegeben wird. |
| [GetName](./getname/) | Der Name des Parameters. |
| [SetName](./setname/) | Der Name des Parameters. |
| [GetCellReference](./getcellreference/) | Zellreferenz, die angibt, welcher Zellenwert für den Abfrageparameter verwendet werden soll. Wird nur verwendet, wenn parameterType = cell. |
| [SetCellReference](./setcellreference/) | Zellreferenz, die angibt, welcher Zellenwert für den Abfrageparameter verwendet werden soll. Wird nur verwendet, wenn parameterType = cell. |
| [GetValue](./getvalue/) | Nicht-ganzzahliger numerischer Wert, ganzzahliger Wert, Zeichenkettenwert oder boolescher Wert, der als Abfrageparameter verwendet wird. Wird nur verwendet, wenn parameterType = value. |
| [SetValue](./setvalue/) | Nicht-ganzzahliger numerischer Wert, ganzzahliger Wert, Zeichenkettenwert oder boolescher Wert, der als Abfrageparameter verwendet wird. Wird nur verwendet, wenn parameterType = value. |
