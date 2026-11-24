---
title: "CellsAI.SpreadsheetQuestion"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CellsAI-Methode. Antwort auf die Frage aus dem Tabellenblatt erhalten, indem TextWriter verwendet wird, um das Ergebnis zu schreiben"
type: docs
url: /de/net/aspose.cells.ai/cellsai/spreadsheetquestion/
---
## SpreadsheetQuestion(string, string, TextWriter) {#spreadsheetquestion_1}

Antwort auf die Frage aus der Tabelle erhalten, wobei TextWriter zum Schreiben des Ergebnisses verwendet wird

```csharp
public Task SpreadsheetQuestion(string path, string question, TextWriter writer)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Pfad | String | der Dateipfad |
| Frage | String | die Frage |
| Schreiber | TextWriter | der TextWriter zum Schreiben des Ergebnisses |

### Siehe auch

* class [CellsAI](../)
* namespace [Aspose.Cells.AI](../../../aspose.cells.ai/)
* assembly [CellsAI](../../../)

---

## SpreadsheetQuestion(string, string) {#spreadsheetquestion}

Antwort auf die Frage aus der Tabelle erhalten

```csharp
public string SpreadsheetQuestion(string path, string question)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Pfad | String | der Dateipfad |
| Frage | String | die Frage |

### Rückgabewert

KI-Abfrageantwort

### Beispiele

```csharp
[C#]
CellsAI cellsAI = new CellsAI(AIRootUrl, AIKey);
String question = @"Which year had the highest total sales revenue?";
String path = "D:\\sales_report.xlsx";
String ret= cellsAI.SpreadsheetQuestion(path, question);
```

### Siehe auch

* class [CellsAI](../)
* namespace [Aspose.Cells.AI](../../../aspose.cells.ai/)
* assembly [CellsAI](../../../)


