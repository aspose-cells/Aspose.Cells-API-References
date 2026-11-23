---
title: "CellsAI.SpreadsheetQuestion"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "CellsAI 方法。使用 TextWriter 将结果写入电子表格以获取问题的答案"
type: docs
url: /zh/net/aspose.cells.ai/cellsai/spreadsheetquestion/
---
## SpreadsheetQuestion(string, string, TextWriter) {#spreadsheetquestion_1}

从电子表格获取问题的答案，使用 TextWriter 写入结果

```csharp
public Task SpreadsheetQuestion(string path, string question, TextWriter writer)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 路径 | String | 文件路径 |
| 问题 | String | 问题 |
| 写入器 | TextWriter | 用于写入结果的 TextWriter |

### 另请参见

* class [CellsAI](../)
* namespace [Aspose.Cells.AI](../../../aspose.cells.ai/)
* assembly [CellsAI](../../../)

---

## SpreadsheetQuestion(string, string) {#spreadsheetquestion}

从电子表格获取问题的答案

```csharp
public string SpreadsheetQuestion(string path, string question)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 路径 | String | 文件路径 |
| 问题 | String | 问题 |

### 返回值

AI 查询响应

### 示例

```csharp
[C#]
CellsAI cellsAI = new CellsAI(AIRootUrl, AIKey);
String question = @"Which year had the highest total sales revenue?";
String path = "D:\\sales_report.xlsx";
String ret= cellsAI.SpreadsheetQuestion(path, question);
```

### 另请参见

* class [CellsAI](../)
* namespace [Aspose.Cells.AI](../../../aspose.cells.ai/)
* assembly [CellsAI](../../../)


