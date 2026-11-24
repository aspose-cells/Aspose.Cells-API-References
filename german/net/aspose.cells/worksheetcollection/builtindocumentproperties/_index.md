---
title: "WorksheetCollection.BuiltInDocumentProperties"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorksheetCollection-Eigenschaft. Gibt eine DocumentProperty‑Sammlung zurück, die alle integrierten Dokumenteigenschaften der Tabelle darstellt"
type: docs
url: /de/net/aspose.cells/worksheetcollection/builtindocumentproperties/
---
## WorksheetCollection.BuiltInDocumentProperties property

Gibt eine [`DocumentProperty`](../../../aspose.cells.properties/documentproperty/)‑Sammlung zurück, die alle integrierten Dokumenteigenschaften der Tabelle darstellt.

```csharp
public BuiltInDocumentPropertyCollection BuiltInDocumentProperties { get; }
```

### Hinweise

Eine neue Eigenschaft kann nicht zur Liste der integrierten Dokumenteigenschaften hinzugefügt werden. Sie können nur eine integrierte Eigenschaft abrufen und ihren Wert ändern. Die folgende Liste enthält die Namen der integrierten Eigenschaften:

Titel

Betreff

Autor

Stichwörter

Kommentare

Vorlage

Letzter Autor

Revisionsnummer

Anwendungsname

Letztes Druckdatum

Erstellungsdatum

Letzte Speicherzeit

Gesamte Bearbeitungszeit

Anzahl der Seiten

Anzahl der Wörter

Anzahl der Zeichen

Sicherheit

Kategorie

Format

Verwalter

Firma

Anzahl der Bytes

Anzahl der Zeilen

Anzahl der Absätze

Anzahl der Folien

Anzahl der Notizen

Anzahl der ausgeblendeten Folien

Anzahl der Multimedia-Clips

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyBuiltInDocumentPropertiesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            DocumentProperty authorProperty = workbook.Worksheets.BuiltInDocumentProperties["Author"];
            authorProperty.Value = "John Smith";
            
            DocumentProperty titleProperty = workbook.Worksheets.BuiltInDocumentProperties["Title"];
            titleProperty.Value = "Sample Document";
            
            Console.WriteLine("Document properties set successfully");
        }
    }
}
```

### Siehe auch

* class [BuiltInDocumentPropertyCollection](../../../aspose.cells.properties/builtindocumentpropertycollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


