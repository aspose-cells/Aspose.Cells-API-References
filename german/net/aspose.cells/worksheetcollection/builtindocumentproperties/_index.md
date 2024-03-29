---
title: BuiltInDocumentProperties
second_title: Aspose.Cells für .NET-API-Referenz
description: Gibt a zurückDocumentPropertyaspose.cells.properties/documentpropertySammlung die alle integrierten Dokumenteigenschaften der Tabelle darstellt.
type: docs
weight: 30
url: /de/net/aspose.cells/worksheetcollection/builtindocumentproperties/
---
## WorksheetCollection.BuiltInDocumentProperties property

Gibt a zurück[`DocumentProperty`](../../../aspose.cells.properties/documentproperty)Sammlung, die alle integrierten Dokumenteigenschaften der Tabelle darstellt.

```csharp
public BuiltInDocumentPropertyCollection BuiltInDocumentProperties { get; }
```

### Bemerkungen

Der Liste der integrierten Dokumenteigenschaften kann keine neue Eigenschaft hinzugefügt werden. Sie können nur eine integrierte Eigenschaft abrufen und ihren Wert ändern. Im Folgenden finden Sie die Namensliste der integrierten Eigenschaften:

Titel

Thema

Autor

Schlüsselwörter

Kommentare

Schablone

Letzter Autor

Revisionsnummer

Anwendungsname

Letztes Druckdatum

Erstellungsdatum

Letzte Speicherzeit

Gesamtbearbeitungszeit

Seitenzahl

Anzahl der Wörter

Anzahl von Charakteren

Sicherheit

Kategorie

Format

Manager

Gesellschaft

Anzahl der Bytes

Anzahl der Zeilen

Anzahl der Absätze

Anzahl der Folien

Anzahl der Notizen

Anzahl der ausgeblendeten Folien

Anzahl der Multimedia-Clips

### Beispiele

```csharp
[C#]
Workbook workbook = new Workbook();
DocumentProperty doc = workbook.Worksheets.BuiltInDocumentProperties["Author"];
doc.Value = "John Smith";

[Visual Basic]
Dim workbook as Workbook = New Workbook()
Dim doc as DocumentProperty = workbook.Worksheets.BuiltInDocumentProperties("Author")
doc.Value = "John Smith"
```

### Siehe auch

* class [BuiltInDocumentPropertyCollection](../../../aspose.cells.properties/builtindocumentpropertycollection)
* class [WorksheetCollection](../../worksheetcollection)
* namensraum [Aspose.Cells](../../worksheetcollection)
* Montage [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
