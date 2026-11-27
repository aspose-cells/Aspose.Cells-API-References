---
title: "GridDesktop.SetCustomResourceManager"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GridDesktop metod. Ställ in anpassad resurshanterare för att implementera användardefinierad lokalisering"
type: docs
url: /sv/net/aspose.cells.griddesktop/griddesktop/setcustomresourcemanager/
---
## GridDesktop.SetCustomResourceManager method

Ställ in anpassad resurs‑hanterare för att implementera användardefinierad lokalisering

```csharp
public void SetCustomResourceManager(ResourceManager customResourceManager)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| customResourceManager | ResourceManager | Den anpassade resurshanteraren. |

### Anmärkningar

För att skapa en anpassad resursfil, följ formatet i GridDesktopResource.resx.

### Exempel

```csharp
[C#]
ResourceManager rm = new ResourceManager("yourapp.customtlocale", Assembly.GetExecutingAssembly());
gridDesktop1.SetCustomResourceManager(rm);
```

### Se även

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


