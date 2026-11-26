---
title: "IGridJsJsonCache.GetCacheKey"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод IGridJsJsonCache. Сгенерировать ключ кэша. Клиенты могут решить, включать ли uid в зависимости от бизнес‑требований. Если важна только имя файла, игнорировать uid и использовать только fileName — рекомендуется для совместного использования кэша между одинаковыми файлами. Если необходимо различать файлы с одинаковым именем, использовать строгий режим с uid."
type: docs
url: /ru/net/aspose.cells.gridjs/igridjsjsoncache/getcachekey/
---
## IGridJsJsonCache.GetCacheKey method

Создать ключ кэша. Клиенты могут решить, включать ли uid в зависимости от бизнес‑требований. - Если важен только имя файла: игнорировать uid и использовать только fileName (рекомендовано, позволяет делиться кэшем между одинаковыми файлами). - Если необходимо различать файлы с одинаковым именем: использовать uid (строгий режим).

```csharp
public string GetCacheKey(string uid, string fileName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| uid | String | Уникальный идентификатор файла (может различаться при каждой загрузке) |
| fileName | String | Исходное имя файла |

### Возвращаемое значение

Ключ кэша

### См. также

* interface [IGridJsJsonCache](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


