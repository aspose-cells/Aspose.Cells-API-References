---
title: "GridJsWorkbook.RedactFile"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод GridJsWorkbook. Выполняет редактирование Excel‑файла на основе массива JSON‑операций."
type: docs
url: /ru/net/aspose.cells.gridjs/gridjsworkbook/redactfile/
---
## GridJsWorkbook.RedactFile method

Выполняет редактирование Excel-файла на основе массива операций JSON.

```csharp
public void RedactFile(string excelFilePath, string uid, string[] arrayOfRedactionOpr)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| excelFilePath | String | Путь к файлу Excel, который будет отредактирован. |
| uid | String | Уникальный идентификатор книги. Если null или пустой, новый uid будет сгенерирован на основе пути к файлу. |
| arrayOfRedactionOpr | String[] | Массив строк JSON, представляющих операции редактирования, которые необходимо применить. |

### Исключения

| исключение | условие |
| --- | --- |
| [GridCellException](../../gridcellexception/) | Выбрасывается, когда во время операции редактирования происходит CellsException. |
| Исключение | Выбрасывается, когда во время операции редактирования происходит общее исключение. |

### См. также

* class [GridJsWorkbook](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


