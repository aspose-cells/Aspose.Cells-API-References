---
title: "SetSecondCommand Метод"
linktitle: "SetSecondCommand"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "SetSecondCommand метод. Инкапсулирует функцию, представляющую setsecondcommand в Go."
type: docs
weight: 200
url: /ru/go-cpp/dbconnection/setsecondcommand/
---

## SetSecondCommand function

Указывает вторую строку текста команды, которая сохраняется при использовании полей PivotTable, основанных на серверных страницах. Для ODBC‑соединений serverCommand обычно представляет более широкий запрос, чем command (в первом отсутствует предложение WHERE). На основе этих двух команд (Command и ServerCommand) можно заполнить пользовательский интерфейс параметров и построить параметризованные запросы.

```go

func (instance *DBConnection) SetSecondCommand(value string)  error

```

## Примечания


## См. также

* Class [DBConnection](../)
* Library [Aspose.Cells for Go](../../)
