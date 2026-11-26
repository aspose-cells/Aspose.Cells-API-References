---
title: "IGridJsService.AddImage"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод IGridJsService. Выполняет операцию добавления изображения из локального файла, принимая байты изображения напрямую"
type: docs
url: /ru/net/aspose.cells.gridjs/igridjsservice/addimage/
---
## AddImage(string, string, string, byte[]) {#addimage}

Выполняет операцию добавления изображения из локального файла, получая байты изображения напрямую.

```csharp
public string AddImage(string p, string uid, string iscontrol, byte[] fileBytes)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| p | String | Параметр JSON‑строка |
| uid | String | Уникальный идентификатор для кэша файла. |
| iscontrol | String | Укажите, является ли это элементом управления. |
| fileBytes | Byte[] | Необработанные байты файла изображения |

### Возвращаемое значение

Результат JSON‑строка

### См. также

* interface [IGridJsService](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)

---

## AddImage(string, string, string, IFormFileCollection) {#addimage_1}

Выполняет операцию добавления изображения из локального файла, используя загруженные файлы формы.

```csharp
public string AddImage(string p, string uid, string iscontrol, IFormFileCollection files)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| p | String | Параметр JSON‑строка |
| uid | String | Уникальный идентификатор для кэша файла. |
| iscontrol | String | Укажите, является ли это элементом управления. |
| файлы | IFormFileCollection | Файл формы изображения |

### Возвращаемое значение

Результат JSON‑строка

### См. также

* interface [IGridJsService](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


