---
title: "CellsAI.SpreadsheetQuestion"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод CellsAI. Получить ответ на вопрос из таблицы, используя TextWriter для записи результата"
type: docs
url: /ru/net/aspose.cells.ai/cellsai/spreadsheetquestion/
---
## SpreadsheetQuestion(string, string, TextWriter) {#spreadsheetquestion_1}

Получить ответ на вопрос из таблицы, используя TextWriter для записи результата

```csharp
public Task SpreadsheetQuestion(string path, string question, TextWriter writer)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| путь | String | путь к файлу |
| вопрос | String | вопрос |
| записыватель | TextWriter | TextWriter для записи результата |

### См. также

* class [CellsAI](../)
* namespace [Aspose.Cells.AI](../../../aspose.cells.ai/)
* assembly [CellsAI](../../../)

---

## SpreadsheetQuestion(string, string) {#spreadsheetquestion}

Получить ответ на вопрос из таблицы

```csharp
public string SpreadsheetQuestion(string path, string question)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| путь | String | путь к файлу |
| вопрос | String | вопрос |

### Возвращаемое значение

Ответ запроса ИИ

### Примеры

```csharp
[C#]
CellsAI cellsAI = new CellsAI(AIRootUrl, AIKey);
String question = @"Which year had the highest total sales revenue?";
String path = "D:\\sales_report.xlsx";
String ret= cellsAI.SpreadsheetQuestion(path, question);
```

### См. также

* class [CellsAI](../)
* namespace [Aspose.Cells.AI](../../../aspose.cells.ai/)
* assembly [CellsAI](../../../)


