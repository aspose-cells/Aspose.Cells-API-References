---
title: "Перечисление HyperlinkLoadMode"
linktitle: "HyperlinkLoadMode"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Перечисление HyperlinkLoadMode. Инкапсулирует объект, представляющий hyperlinkloadmode в Go."
type: docs
weight: 200
url: /ru/go-cpp/hyperlinkloadmode/
---

## HyperlinkLoadMode Enum

Указывает, как обрабатываются гиперссылки при загрузке HTML.

```go

type HyperlinkLoadMode int32


```

## Поля

| Поле | Описание |
| --- | --- |
| [Normal](./normal/) | Загружается только первая гиперссылка в ячейке, последующие игнорируются. |
| [AllowMultiple](./allowmultiple/) | Все гиперссылки в ячейке добавляются в <see cref="Worksheet.Hyperlinks"/>. Обратите внимание, что MS Excel поддерживает только одну гиперссылку на ячейку, поэтому эта опция может создавать файлы, которые Excel не сможет полностью отобразить. |
