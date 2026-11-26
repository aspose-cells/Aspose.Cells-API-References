---
title: "CellsAI.SpreadsheetQuestion"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método CellsAI. Obtener respuesta de la pregunta de la hoja de cálculo usando TextWriter para escribir el resultado"
type: docs
url: /es/net/aspose.cells.ai/cellsai/spreadsheetquestion/
---
## SpreadsheetQuestion(string, string, TextWriter) {#spreadsheetquestion_1}

Obtener respuesta de la pregunta desde la hoja de cálculo, usando TextWriter para escribir el resultado

```csharp
public Task SpreadsheetQuestion(string path, string question, TextWriter writer)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ruta | String | la ruta del archivo |
| pregunta | String | la pregunta |
| escritor | TextWriter | el TextWriter para escribir el resultado |

### Ver también

* class [CellsAI](../)
* namespace [Aspose.Cells.AI](../../../aspose.cells.ai/)
* assembly [CellsAI](../../../)

---

## SpreadsheetQuestion(string, string) {#spreadsheetquestion}

Obtener respuesta de la pregunta desde la hoja de cálculo

```csharp
public string SpreadsheetQuestion(string path, string question)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ruta | String | la ruta del archivo |
| pregunta | String | la pregunta |

### Valor de retorno

respuesta de consulta de IA

### Ejemplos

```csharp
[C#]
CellsAI cellsAI = new CellsAI(AIRootUrl, AIKey);
String question = @"Which year had the highest total sales revenue?";
String path = "D:\\sales_report.xlsx";
String ret= cellsAI.SpreadsheetQuestion(path, question);
```

### Ver también

* class [CellsAI](../)
* namespace [Aspose.Cells.AI](../../../aspose.cells.ai/)
* assembly [CellsAI](../../../)


