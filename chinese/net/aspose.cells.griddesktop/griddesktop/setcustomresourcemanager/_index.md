---
title: "GridDesktop.SetCustomResourceManager"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "GridDesktop 方法。设置自定义资源管理器以实现用户定义的本地化"
type: docs
url: /zh/net/aspose.cells.griddesktop/griddesktop/setcustomresourcemanager/
---
## GridDesktop.SetCustomResourceManager method

设置自定义资源管理器以实现用户定义的本地化

```csharp
public void SetCustomResourceManager(ResourceManager customResourceManager)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| customResourceManager | ResourceManager | 自定义资源管理器。 |

### 备注

要创建自定义资源文件，请遵循 GridDesktopResource.resx 中的格式。

### 示例

```csharp
[C#]
ResourceManager rm = new ResourceManager("yourapp.customtlocale", Assembly.GetExecutingAssembly());
gridDesktop1.SetCustomResourceManager(rm);
```

### 另请参见

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


