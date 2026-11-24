---
title: "Workbook.BuiltInDocumentProperties"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Eigenschaft. Gibt eine DocumentProperty-Sammlung zurück, die alle integrierten Dokumenteigenschaften der Tabelle darstellt"
type: docs
url: /de/net/aspose.cells/workbook/builtindocumentproperties/
---
## Workbook.BuiltInDocumentProperties property

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
    public class WorkbookPropertyBuiltInDocumentPropertiesDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf und Ändern integrierter Dokumenteigenschaften
            DocumentProperty authorProperty = workbook.BuiltInDocumentProperties["Author"];
            authorProperty.Value = "John Smith";
            
            DocumentProperty titleProperty = workbook.BuiltInDocumentProperties["Title"];
            titleProperty.Value = "Sample Workbook";
            
            // Die geänderten Eigenschaften anzeigen
            Console.WriteLine("Author: " + workbook.BuiltInDocumentProperties["Author"].Value);
            Console.WriteLine("Title: " + workbook.BuiltInDocumentProperties["Title"].Value);
        }
    }
}
```

### Siehe auch

* class [BuiltInDocumentPropertyCollection](../../../aspose.cells.properties/builtindocumentpropertycollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


