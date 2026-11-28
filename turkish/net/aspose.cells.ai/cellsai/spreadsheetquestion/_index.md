---
title: "CellsAI.SpreadsheetQuestion"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CellsAI yöntemi. Sorunun cevabını elektronik tablodan al, sonucu yazmak için TextWriter kullan"
type: docs
url: /tr/net/aspose.cells.ai/cellsai/spreadsheetquestion/
---
## SpreadsheetQuestion(string, string, TextWriter) {#spreadsheetquestion_1}

Elektronik tablodan sorunun cevabını al, sonucu yazmak için TextWriter kullan

```csharp
public Task SpreadsheetQuestion(string path, string question, TextWriter writer)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yol | String | dosya yolu |
| soru | String | soru |
| yazıcı | TextWriter | sonucu yazmak için TextWriter |

### Ayrıca Bakınız

* class [CellsAI](../)
* namespace [Aspose.Cells.AI](../../../aspose.cells.ai/)
* assembly [CellsAI](../../../)

---

## SpreadsheetQuestion(string, string) {#spreadsheetquestion}

Elektronik tablodan sorunun cevabını al

```csharp
public string SpreadsheetQuestion(string path, string question)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yol | String | dosya yolu |
| soru | String | soru |

### Dönüş Değeri

AI sorgu yanıtı

### Örnekler

```csharp
[C#]
CellsAI cellsAI = new CellsAI(AIRootUrl, AIKey);
String question = @"Which year had the highest total sales revenue?";
String path = "D:\\sales_report.xlsx";
String ret= cellsAI.SpreadsheetQuestion(path, question);
```

### Ayrıca Bakınız

* class [CellsAI](../)
* namespace [Aspose.Cells.AI](../../../aspose.cells.ai/)
* assembly [CellsAI](../../../)


