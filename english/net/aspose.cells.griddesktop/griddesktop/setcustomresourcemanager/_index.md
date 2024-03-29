---
title: GridDesktop.SetCustomResourceManager
second_title: Aspose.Cells for .NET API Reference
description: GridDesktop method. Set custom resource manager to implement user defined localization
type: docs
url: /net/aspose.cells.griddesktop/griddesktop/setcustomresourcemanager/
---
## GridDesktop.SetCustomResourceManager method

Set custom resource manager to implement user defined localization

```csharp
public void SetCustomResourceManager(ResourceManager customResourceManager)
```

| Parameter | Type | Description |
| --- | --- | --- |
| customResourceManager | ResourceManager | the custom resource manager. |

### Remarks

To create a customized resource file ,Please follow the format in GridDesktopResource.resx.

### Examples

```csharp
[C#]
ResourceManager rm = new ResourceManager("yourapp.customtlocale", Assembly.GetExecutingAssembly());
gridDesktop1.SetCustomResourceManager(rm);
```

### See Also

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


