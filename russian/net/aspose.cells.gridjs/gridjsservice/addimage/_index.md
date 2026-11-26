---
title: "GridJsService.AddImage"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод GridJsService. Выполняет добавление изображения из локального файла; байты файла поступают из JS FormData или любого хоста."
type: docs
url: /ru/net/aspose.cells.gridjs/gridjsservice/addimage/
---
## AddImage(string, string, string, byte[]) {#addimage}

Выполняет операцию добавления изображения из локального файла (байты файла поступают из JS FormData или любого хоста).

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

* class [GridJsService](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)

---

## AddImage(string, string, string, IFormFileCollection) {#addimage_1}

Выполняет операцию добавления изображения из локального файла.

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

* class [GridJsService](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


