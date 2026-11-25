---
title: "GridDesktop.SetCustomResourceManager"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo GridDesktop. Imposta il gestore di risorse personalizzato per implementare la localizzazione definita dall'utente"
type: docs
url: /it/net/aspose.cells.griddesktop/griddesktop/setcustomresourcemanager/
---
## GridDesktop.SetCustomResourceManager method

Imposta un gestore di risorse personalizzato per implementare la localizzazione definita dall'utente

```csharp
public void SetCustomResourceManager(ResourceManager customResourceManager)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| customResourceManager | ResourceManager | il gestore di risorse personalizzato. |

### Osservazioni

Per creare un file di risorse personalizzato, seguire il formato in GridDesktopResource.resx.

### Esempi

```csharp
[C#]
ResourceManager rm = new ResourceManager("yourapp.customtlocale", Assembly.GetExecutingAssembly());
gridDesktop1.SetCustomResourceManager(rm);
```

### Vedi anche

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


