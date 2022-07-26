---
title: DBConnection
second_title: Aspose.Cells for .NET API Referansı
description: Bir ODBC veya OLE DB harici veri bağlantısıyla ilişkili tüm özellikleri belirtir.
type: docs
weight: 3280
url: /tr/net/aspose.cells.externalconnections/dbconnection/
---
## DBConnection class

Bir ODBC veya OLE DB harici veri bağlantısıyla ilişkili tüm özellikleri belirtir.

```csharp
public class DBConnection : ExternalConnection
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [BackgroundRefresh](../../aspose.cells.externalconnections/externalconnection/backgroundrefresh) { get; set; } | Bağlantının arka planda (eşzamansız olarak) yenilenip yenilenmeyeceğini gösterir. bağlantının tercih edilen kullanımı arka planda zaman uyumsuz olarak yenilemekse true ; false, bağlantının tercih edilen kullanımı ön planda eşzamanlı olarak yenilemekse. |
| [Command](../../aspose.cells.externalconnections/dbconnection/command) { get; set; } | Veriyi almak için harici kaynakla etkileşime girecek veri sağlayıcı API'sine geçirilecek veritabanı komutunu içeren dize |
| [CommandType](../../aspose.cells.externalconnections/dbconnection/commandtype) { get; set; } | OLE DB komut türünü belirtir. 1. Sorgu bir küp name belirtir 2. Sorgu bir SQL deyimi belirtir 3. Sorgu bir tablo adı belirtir 4. Sorgu, varsayılan bilgilerin verildiğini belirtir ve nasıl yorumlanacağı sağlayıcıya bağlıdır. 5. Sorgu karşıdır web tabanlı bir Liste Veri Sağlayıcısı. |
| [ConnectionDescription](../../aspose.cells.externalconnections/externalconnection/connectiondescription) { get; set; } | Bu bağlantı için kullanıcı tanımını belirtir |
| [ConnectionId](../../aspose.cells.externalconnections/externalconnection/connectionid) { get; } | Bu bağlantının benzersiz tanımlayıcısını belirtir. |
| [ConnectionInfo](../../aspose.cells.externalconnections/dbconnection/connectioninfo) { get; set; } | Bağlantı bilgisi dizesi, bir OLE DB veya ODBC veri kaynağıyla bağlantı kurmak için kullanılır. |
| [CredentialsMethodType](../../aspose.cells.externalconnections/externalconnection/credentialsmethodtype) { get; set; } | Bağlantı kurulurken (veya yeniden kurulurken) kullanılacak kimlik doğrulama yöntemini belirtir. |
| [Id](../../aspose.cells.externalconnections/externalconnection/id) { get; } | Bağlantının kimliğini alır. |
| [IsDeleted](../../aspose.cells.externalconnections/externalconnection/isdeleted) { get; set; } | İlişkili çalışma kitabı bağlantısının silinip silinmediğini gösterir. the bağlantısı silinmişse true ; aksi takdirde, false. |
| [IsNew](../../aspose.cells.externalconnections/externalconnection/isnew) { get; set; } | Bağlantı ilk kez yenilenmediyse doğrudur; aksi halde yanlış. Bu durum, kullanıcı, bir sorgunun dönüşü tamamlanmadan önce dosyayı kaydettiğinde ortaya çıkabilir. |
| [KeepAlive](../../aspose.cells.externalconnections/externalconnection/keepalive) { get; set; } | Elektronik tablo uygulamasının bağlantısını açık tutmak için çaba göstermesi gerektiğinde doğrudur. Yanlış olduğunda, uygulama bilgilerini aldıktan sonra bağlantıyı kapatmalıdır. |
| [Name](../../aspose.cells.externalconnections/externalconnection/name) { get; set; } | Bağlantının adını belirtir. Her bağlantının benzersiz bir adı olmalıdır. |
| [OdcFile](../../aspose.cells.externalconnections/externalconnection/odcfile) { get; set; } | Bu bağlantının oluşturulduğu harici bağlantı dosyasının tam yolunu belirtir. Verileri yenileme girişimi sırasında bir bağlantı başarısız olursa ve reconnectionMethod=1, ise, elektronik tablo uygulaması, çalışma kitabına katıştırılmış bağlantı nesnesi yerine harici bağlantı dosyasındaki bilgileri kullanmayı tekrar deneyecektir. |
| [OnlyUseConnectionFile](../../aspose.cells.externalconnections/externalconnection/onlyuseconnectionfile) { get; set; } | Elektronik tablo uygulamasının, bağlantı yenilendiğinde odcFile özniteliği tarafından belirtilen harici bağlantı dosyasındaki bağlantı bilgilerini her zaman ve yalnızca kullanması gerekip gerekmediğini gösterir. Yanlışsa, elektronik tablo uygulaması , reconnectionMethod özniteliği tarafından belirtilen prosedürü izlemelidir. |
| [Parameters](../../aspose.cells.externalconnections/externalconnection/parameters) { get; } | Alır[`ConnectionParameterCollection`](../connectionparametercollection) bir ODBC veya web sorgusu için. |
| override [PowerQueryFormula](../../aspose.cells.externalconnections/dbconnection/powerqueryformula) { get; } | Güçlü sorgu formülünün tanımını alır. |
| [ReconnectionMethodType](../../aspose.cells.externalconnections/externalconnection/reconnectionmethodtype) { get; set; } | Bir bağlantı başarısız olduğunda elektronik tablo uygulamasının ne yapması gerektiğini belirtir. Varsayılan değer, ReConnectionMethodType.Required. 'dir. |
| [RefreshInternal](../../aspose.cells.externalconnections/externalconnection/refreshinternal) { get; set; } | Bağlantının otomatik olarak yenilenmesi arasındaki dakika sayısını belirtir. |
| [RefreshOnLoad](../../aspose.cells.externalconnections/externalconnection/refreshonload) { get; set; } | Dosya açılırken bu bağlantının yenilenmesi gerekiyorsa doğrudur; aksi takdirde, false. |
| [SaveData](../../aspose.cells.externalconnections/externalconnection/savedata) { get; set; } | Bir tabloyu doldurmak için bağlantı üzerinden alınan dış veriler çalışma kitabıyla birlikte kaydedilecekse doğrudur; aksi halde yanlış. |
| [SavePassword](../../aspose.cells.externalconnections/externalconnection/savepassword) { get; set; } | Parola bağlantı dizesinin bir parçası olarak kaydedilecekse doğru; aksi takdirde, False. |
| [SeverCommand](../../aspose.cells.externalconnections/dbconnection/severcommand) { get; set; } | PivotTable sunucusu tabanlı sayfa alanları kullanımdayken kalıcı olan ikinci bir komut metni dizesini belirtir. ODBC bağlantıları için, serverCommand genellikle komuttan daha geniş bir sorgudur (öncesinde WHERE yan tümcesi yoktur). Bu 2 komuta (Komut ve SunucuKomutu) dayanarak, parametre kullanıcı arayüzü doldurulabilir ve parametreli sorgular oluşturulabilir |
| [SourceFile](../../aspose.cells.externalconnections/externalconnection/sourcefile) { get; set; } | Harici veri kaynağı dosya tabanlı olduğunda kullanılır. Böyle bir veri kaynağına bağlantı başarısız olduğunda, elektronik tablo uygulaması doğrudan bu dosyaya bağlanmayı dener. URI veya sisteme özgü dosya yolu gösteriminde ifade edilebilir. |
| [SSOId](../../aspose.cells.externalconnections/externalconnection/ssoid) { get; set; } | Ara elektronik tabloML sunucusu ile harici veri kaynağı arasında kimlik doğrulaması için kullanılan Tekli Oturum Açma (SSO) tanımlayıcısı. |
| [Type](../../aspose.cells.externalconnections/externalconnection/type) { get; set; } | Harici bağlantı DataSource türünü alır veya ayarlar. |

### Ayrıca bakınız

* class [ExternalConnection](../externalconnection)
* ad alanı [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections)
* toplantı [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
