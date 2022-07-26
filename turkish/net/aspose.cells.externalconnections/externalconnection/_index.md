---
title: ExternalConnection
second_title: Aspose.Cells for .NET API Referansı
description: Harici bir veri bağlantısını belirtir
type: docs
weight: 3290
url: /tr/net/aspose.cells.externalconnections/externalconnection/
---
## ExternalConnection class

Harici bir veri bağlantısını belirtir

```csharp
public abstract class ExternalConnection
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [BackgroundRefresh](../../aspose.cells.externalconnections/externalconnection/backgroundrefresh) { get; set; } | Bağlantının arka planda (eşzamansız olarak) yenilenip yenilenmeyeceğini gösterir. bağlantının tercih edilen kullanımı arka planda zaman uyumsuz olarak yenilemekse true ; false, bağlantının tercih edilen kullanımı ön planda eşzamanlı olarak yenilemekse. |
| [ConnectionDescription](../../aspose.cells.externalconnections/externalconnection/connectiondescription) { get; set; } | Bu bağlantı için kullanıcı tanımını belirtir |
| [ConnectionId](../../aspose.cells.externalconnections/externalconnection/connectionid) { get; } | Bu bağlantının benzersiz tanımlayıcısını belirtir. |
| [CredentialsMethodType](../../aspose.cells.externalconnections/externalconnection/credentialsmethodtype) { get; set; } | Bağlantı kurulurken (veya yeniden kurulurken) kullanılacak kimlik doğrulama yöntemini belirtir. |
| [Id](../../aspose.cells.externalconnections/externalconnection/id) { get; } | Bağlantının kimliğini alır. |
| [IsDeleted](../../aspose.cells.externalconnections/externalconnection/isdeleted) { get; set; } | İlişkili çalışma kitabı bağlantısının silinip silinmediğini gösterir. the bağlantısı silinmişse true ; aksi takdirde, false. |
| [IsNew](../../aspose.cells.externalconnections/externalconnection/isnew) { get; set; } | Bağlantı ilk kez yenilenmediyse doğrudur; aksi halde yanlış. Bu durum, kullanıcı, bir sorgunun dönüşü tamamlanmadan önce dosyayı kaydettiğinde ortaya çıkabilir. |
| [KeepAlive](../../aspose.cells.externalconnections/externalconnection/keepalive) { get; set; } | Elektronik tablo uygulamasının bağlantısını açık tutmak için çaba göstermesi gerektiğinde doğrudur. Yanlış olduğunda, uygulama bilgilerini aldıktan sonra bağlantıyı kapatmalıdır. |
| [Name](../../aspose.cells.externalconnections/externalconnection/name) { get; set; } | Bağlantının adını belirtir. Her bağlantının benzersiz bir adı olmalıdır. |
| [OdcFile](../../aspose.cells.externalconnections/externalconnection/odcfile) { get; set; } | Bu bağlantının oluşturulduğu harici bağlantı dosyasının tam yolunu belirtir. Verileri yenileme girişimi sırasında bir bağlantı başarısız olursa ve reconnectionMethod=1, ise, elektronik tablo uygulaması, çalışma kitabına katıştırılmış bağlantı nesnesi yerine harici bağlantı dosyasındaki bilgileri kullanmayı tekrar deneyecektir. |
| [OnlyUseConnectionFile](../../aspose.cells.externalconnections/externalconnection/onlyuseconnectionfile) { get; set; } | Elektronik tablo uygulamasının, bağlantı yenilendiğinde odcFile özniteliği tarafından belirtilen harici bağlantı dosyasındaki bağlantı bilgilerini her zaman ve yalnızca kullanması gerekip gerekmediğini gösterir. Yanlışsa, elektronik tablo uygulaması , reconnectionMethod özniteliği tarafından belirtilen prosedürü izlemelidir. |
| [Parameters](../../aspose.cells.externalconnections/externalconnection/parameters) { get; } | Alır[`ConnectionParameterCollection`](../connectionparametercollection) bir ODBC veya web sorgusu için. |
| virtual [PowerQueryFormula](../../aspose.cells.externalconnections/externalconnection/powerqueryformula) { get; } | Güçlü sorgu formülünün tanımını alır. |
| [ReconnectionMethodType](../../aspose.cells.externalconnections/externalconnection/reconnectionmethodtype) { get; set; } | Bir bağlantı başarısız olduğunda elektronik tablo uygulamasının ne yapması gerektiğini belirtir. Varsayılan değer, ReConnectionMethodType.Required. 'dir. |
| [RefreshInternal](../../aspose.cells.externalconnections/externalconnection/refreshinternal) { get; set; } | Bağlantının otomatik olarak yenilenmesi arasındaki dakika sayısını belirtir. |
| [RefreshOnLoad](../../aspose.cells.externalconnections/externalconnection/refreshonload) { get; set; } | Dosya açılırken bu bağlantının yenilenmesi gerekiyorsa doğrudur; aksi takdirde, false. |
| [SaveData](../../aspose.cells.externalconnections/externalconnection/savedata) { get; set; } | Bir tabloyu doldurmak için bağlantı üzerinden alınan dış veriler çalışma kitabıyla birlikte kaydedilecekse doğrudur; aksi halde yanlış. |
| [SavePassword](../../aspose.cells.externalconnections/externalconnection/savepassword) { get; set; } | Parola bağlantı dizesinin bir parçası olarak kaydedilecekse doğru; aksi takdirde, False. |
| [SourceFile](../../aspose.cells.externalconnections/externalconnection/sourcefile) { get; set; } | Harici veri kaynağı dosya tabanlı olduğunda kullanılır. Böyle bir veri kaynağına bağlantı başarısız olduğunda, elektronik tablo uygulaması doğrudan bu dosyaya bağlanmayı dener. URI veya sisteme özgü dosya yolu gösteriminde ifade edilebilir. |
| [SSOId](../../aspose.cells.externalconnections/externalconnection/ssoid) { get; set; } | Ara elektronik tabloML sunucusu ile harici veri kaynağı arasında kimlik doğrulaması için kullanılan Tekli Oturum Açma (SSO) tanımlayıcısı. |
| [Type](../../aspose.cells.externalconnections/externalconnection/type) { get; set; } | Harici bağlantı DataSource türünü alır veya ayarlar. |

### Ayrıca bakınız

* ad alanı [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections)
* toplantı [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
