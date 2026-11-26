---
title: "GridDesktop.SetCustomResourceManager"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de GridDesktop. Establece un administrador de recursos personalizado para implementar la localización definida por el usuario"
type: docs
url: /es/net/aspose.cells.griddesktop/griddesktop/setcustomresourcemanager/
---
## GridDesktop.SetCustomResourceManager method

Establece un gestor de recursos personalizado para implementar la localización definida por el usuario

```csharp
public void SetCustomResourceManager(ResourceManager customResourceManager)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| customResourceManager | ResourceManager | el administrador de recursos personalizado. |

### Observaciones

Para crear un archivo de recursos personalizado, siga el formato en GridDesktopResource.resx.

### Ejemplos

```csharp
[C#]
ResourceManager rm = new ResourceManager("yourapp.customtlocale", Assembly.GetExecutingAssembly());
gridDesktop1.SetCustomResourceManager(rm);
```

### Ver también

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


