---
title: "CellsAI.SpreadsheetQuestion"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CellsAI method. Hämta svaret på frågan från kalkylbladet med TextWriter för att skriva resultatet"
type: docs
url: /sv/net/aspose.cells.ai/cellsai/spreadsheetquestion/
---
## SpreadsheetQuestion(string, string, TextWriter) {#spreadsheetquestion_1}

Hämta svar på frågan från kalkylbladet, med TextWriter för att skriva resultatet

```csharp
public Task SpreadsheetQuestion(string path, string question, TextWriter writer)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sökväg | String | filvägen |
| fråga | String | frågan |
| skrivare | TextWriter | TextWriter för att skriva resultatet |

### Se även

* class [CellsAI](../)
* namespace [Aspose.Cells.AI](../../../aspose.cells.ai/)
* assembly [CellsAI](../../../)

---

## SpreadsheetQuestion(string, string) {#spreadsheetquestion}

Hämta svar på frågan från kalkylbladet

```csharp
public string SpreadsheetQuestion(string path, string question)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sökväg | String | filvägen |
| fråga | String | frågan |

### Returvärde

AI-frågesvar

### Exempel

```csharp
[C#]
CellsAI cellsAI = new CellsAI(AIRootUrl, AIKey);
String question = @"Which year had the highest total sales revenue?";
String path = "D:\\sales_report.xlsx";
String ret= cellsAI.SpreadsheetQuestion(path, question);
```

### Se även

* class [CellsAI](../)
* namespace [Aspose.Cells.AI](../../../aspose.cells.ai/)
* assembly [CellsAI](../../../)


