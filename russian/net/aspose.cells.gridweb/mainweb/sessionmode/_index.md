---
title: "MainWeb.SessionMode"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство MainWeb. Получает или задает режим сеанса сетки"
type: docs
url: /ru/net/aspose.cells.gridweb/mainweb/sessionmode/
---
## MainWeb.SessionMode property

Получает или задает режим сеанса сетки.

```csharp
public SessionMode SessionMode { get; set; }
```

### Примечания

Существует 4 типа режима сеанса: 1. Session(default): использовать системный сеанс для хранения данных листа. Обычно asp.net использует состояние сеанса InProc. Сетка также поддерживает "StateServer" внешнее состояние сеанса и состояние сеанса SQLServer. 2. ViewState: использовать viewstate страницы для хранения данных листа. 3. Custom: использовать события LoadCustomData и SheetDataUpdated для сохранения/восстановления данных листа. 4. File: сохранять/восстанавливать данные листа в SessionStorePath. это рекомендуемый способ и может постоянно хранить файл. При использовании SessionMode.ViewState сетка будет сохранять некоторые данные в viewstate страницы. Это уменьшит использование памяти сервера, но размер страницы увеличится и это повлияет на общую производительность.

### Примеры

```csharp
[C#]
	GridWeb1.SessionMode = SessionMode.ViewState;
	
[Visual Basic]
	GridWeb1.SessionMode = SessionMode.ViewState
```

### См. также

* enum [SessionMode](../../sessionmode/)
* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)


