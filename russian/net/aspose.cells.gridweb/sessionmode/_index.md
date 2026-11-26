---
title: "Перечисление SessionMode"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.GridWeb.SessionMode. Представляет режим сеанса сетки"
type: docs
url: /ru/net/aspose.cells.gridweb/sessionmode/
---
## SessionMode enumeration

Представляет режим сеанса сетки.

```csharp
public enum SessionMode
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Session | `0` | Использует системный сеанс для автоматического сохранения/восстановления данных листа сетки. |
| ViewState | `1` | Использует viewstate страницы для автоматического сохранения/восстановления данных листа сетки. |
| Custom | `2` | Использует событие LoadCustomData для ручной загрузки данных листа сетки. И использует событие SheetDataUpdated для сохранения данных листа сетки. |
| File | `3` | Использует системный файл для автоматического сохранения/восстановления данных листа сетки, пользователь должен установить SessionStorePath для указания каталога файлов. |

### См. также

* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


