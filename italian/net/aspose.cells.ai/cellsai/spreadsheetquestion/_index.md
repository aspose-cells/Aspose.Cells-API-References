---
title: "CellsAI.SpreadsheetQuestion"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo CellsAI. Ottieni la risposta della domanda dal foglio di calcolo usando TextWriter per scrivere il risultato"
type: docs
url: /it/net/aspose.cells.ai/cellsai/spreadsheetquestion/
---
## SpreadsheetQuestion(string, string, TextWriter) {#spreadsheetquestion_1}

Ottieni risposta alla domanda dal foglio di calcolo, usando TextWriter per scrivere il risultato

```csharp
public Task SpreadsheetQuestion(string path, string question, TextWriter writer)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| percorso | String | il percorso del file |
| domanda | String | la domanda |
| scrittore | TextWriter | Il TextWriter per scrivere il risultato |

### Vedi anche

* class [CellsAI](../)
* namespace [Aspose.Cells.AI](../../../aspose.cells.ai/)
* assembly [CellsAI](../../../)

---

## SpreadsheetQuestion(string, string) {#spreadsheetquestion}

Ottieni risposta alla domanda dal foglio di calcolo

```csharp
public string SpreadsheetQuestion(string path, string question)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| percorso | String | il percorso del file |
| domanda | String | la domanda |

### Valore di ritorno

Risposta della query AI

### Esempi

```csharp
[C#]
CellsAI cellsAI = new CellsAI(AIRootUrl, AIKey);
String question = @"Which year had the highest total sales revenue?";
String path = "D:\\sales_report.xlsx";
String ret= cellsAI.SpreadsheetQuestion(path, question);
```

### Vedi anche

* class [CellsAI](../)
* namespace [Aspose.Cells.AI](../../../aspose.cells.ai/)
* assembly [CellsAI](../../../)


