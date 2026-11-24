---
title: "GridDesktop.SetCustomResourceManager"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GridDesktop-Methode. Legen Sie einen benutzerdefinierten Ressourcen-Manager fest, um benutzerdefinierte Lokalisierung zu implementieren"
type: docs
url: /de/net/aspose.cells.griddesktop/griddesktop/setcustomresourcemanager/
---
## GridDesktop.SetCustomResourceManager method

Benutzerdefinierten Ressourcen-Manager festlegen, um benutzerdefinierte Lokalisierung zu implementieren

```csharp
public void SetCustomResourceManager(ResourceManager customResourceManager)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| customResourceManager | ResourceManager | der benutzerdefinierte Ressourcen-Manager. |

### Hinweise

Um eine benutzerdefinierte Ressourcendatei zu erstellen, folgen Sie bitte dem Format in GridDesktopResource.resx.

### Beispiele

```csharp
[C#]
ResourceManager rm = new ResourceManager("yourapp.customtlocale", Assembly.GetExecutingAssembly());
gridDesktop1.SetCustomResourceManager(rm);
```

### Siehe auch

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


