---
title: "GridDesktop.SetCustomResourceManager"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GridDesktop yöntemi. Kullanıcı tanımlı yerelleştirmeyi uygulamak için özel kaynak yöneticisini ayarlar"
type: docs
url: /tr/net/aspose.cells.griddesktop/griddesktop/setcustomresourcemanager/
---
## GridDesktop.SetCustomResourceManager method

Kullanıcı tanımlı yerelleştirmeyi uygulamak için özel kaynak yöneticisi ayarlar

```csharp
public void SetCustomResourceManager(ResourceManager customResourceManager)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| customResourceManager | ResourceManager | özel kaynak yöneticisi. |

### Açıklamalar

Özelleştirilmiş bir kaynak dosyası oluşturmak için, lütfen GridDesktopResource.resx içindeki formatı izleyin.

### Örnekler

```csharp
[C#]
ResourceManager rm = new ResourceManager("yourapp.customtlocale", Assembly.GetExecutingAssembly());
gridDesktop1.SetCustomResourceManager(rm);
```

### Ayrıca Bakınız

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


