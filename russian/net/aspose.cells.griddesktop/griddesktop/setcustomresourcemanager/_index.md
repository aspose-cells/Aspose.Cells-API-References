---
title: "GridDesktop.SetCustomResourceManager"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод GridDesktop. Устанавливает пользовательский менеджер ресурсов для реализации локализации, определяемой пользователем"
type: docs
url: /ru/net/aspose.cells.griddesktop/griddesktop/setcustomresourcemanager/
---
## GridDesktop.SetCustomResourceManager method

Установить пользовательский менеджер ресурсов для реализации пользовательской локализации

```csharp
public void SetCustomResourceManager(ResourceManager customResourceManager)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| customResourceManager | ResourceManager | этот пользовательский менеджер ресурсов. |

### Примечания

Чтобы создать пользовательский файл ресурсов, следуйте формату в GridDesktopResource.resx.

### Примеры

```csharp
[C#]
ResourceManager rm = new ResourceManager("yourapp.customtlocale", Assembly.GetExecutingAssembly());
gridDesktop1.SetCustomResourceManager(rm);
```

### См. также

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


