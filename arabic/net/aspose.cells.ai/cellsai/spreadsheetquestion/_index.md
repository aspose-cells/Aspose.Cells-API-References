---
title: "CellsAI.SpreadsheetQuestion"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة CellsAI. الحصول على إجابة السؤال من جدول البيانات باستخدام TextWriter لكتابة النتيجة"
type: docs
url: /ar/net/aspose.cells.ai/cellsai/spreadsheetquestion/
---
## SpreadsheetQuestion(string, string, TextWriter) {#spreadsheetquestion_1}

الحصول على إجابة السؤال من جدول البيانات، باستخدام TextWriter لكتابة النتيجة

```csharp
public Task SpreadsheetQuestion(string path, string question, TextWriter writer)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المسار | String | مسار الملف |
| سؤال | String | السؤال |
| كاتب | TextWriter | TextWriter لكتابة النتيجة |

### انظر أيضًا

* class [CellsAI](../)
* namespace [Aspose.Cells.AI](../../../aspose.cells.ai/)
* assembly [CellsAI](../../../)

---

## SpreadsheetQuestion(string, string) {#spreadsheetquestion}

الحصول على إجابة السؤال من جدول البيانات

```csharp
public string SpreadsheetQuestion(string path, string question)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المسار | String | مسار الملف |
| سؤال | String | السؤال |

### قيمة الإرجاع

استجابة استعلام AI

### أمثلة

```csharp
[C#]
CellsAI cellsAI = new CellsAI(AIRootUrl, AIKey);
String question = @"Which year had the highest total sales revenue?";
String path = "D:\\sales_report.xlsx";
String ret= cellsAI.SpreadsheetQuestion(path, question);
```

### انظر أيضًا

* class [CellsAI](../)
* namespace [Aspose.Cells.AI](../../../aspose.cells.ai/)
* assembly [CellsAI](../../../)


