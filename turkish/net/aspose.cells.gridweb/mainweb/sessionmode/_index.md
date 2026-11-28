---
title: "MainWeb.SessionMode"
second_title: "Aspose.Cells için .NET API Referansı"
description: "MainWeb özelliği. Izgaranın oturum modunu alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.gridweb/mainweb/sessionmode/
---
## MainWeb.SessionMode property

Izgaranın oturum modunu alır veya ayarlar.

```csharp
public SessionMode SessionMode { get; set; }
```

### Açıklamalar

4 tür oturum modu vardır: 1. Session (varsayılan): Sayfa verilerini depolamak için sistem oturumu kullanılır. Genel olarak asp.net InProc oturum durumunu kullanır. Izgara ayrıca "StateServer" dış süreç oturum durumu ve SQLServer oturum durumunu da destekler. 2. ViewState: Sayfa viewstate'ini kullanarak sayfa verileri depolanır. 3. Custom: LoadCustomData ve SheetDataUpdated olaylarını kullanarak sayfa verileri depolanır/kurtarılır. 4. File: Sayfa verileri SessionStorePath içinde depolanır/kurtarılır. Bu önerilen yoldur ve dosya her zaman saklanabilir. SessionMode.ViewState kullanıldığında, ızgara bazı verileri sayfanın view state'ine depolar. Bu, sunucunun bellek kullanımını azaltır, ancak sayfanın boyutu büyür ve genel performansı etkiler.

### Örnekler

```csharp
[C#]
	GridWeb1.SessionMode = SessionMode.ViewState;
	
[Visual Basic]
	GridWeb1.SessionMode = SessionMode.ViewState
```

### Ayrıca Bakınız

* enum [SessionMode](../../sessionmode/)
* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)


