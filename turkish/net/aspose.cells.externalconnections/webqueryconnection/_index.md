---
title: WebQueryConnection
second_title: Aspose.Cells for .NET API Referansı
description: Bir web sorgusu kaynağının özelliklerini belirtir. Bir web sorgusu HTML tablolarından verileri alır ve ayrıca parametreler ve parametre öğeleri dahil olmak üzere tarafından HTML oluşturulurken web sunucusu tarafından işlenecek HTTP Get parametrelerini sağlayabilir.
type: docs
weight: 3350
url: /tr/net/aspose.cells.externalconnections/webqueryconnection/
---
## WebQueryConnection class

Bir web sorgusu kaynağının özelliklerini belirtir. Bir web sorgusu, HTML tablolarından verileri alır ve ayrıca parametreler ve parametre öğeleri dahil olmak üzere tarafından HTML oluşturulurken web sunucusu tarafından işlenecek HTTP "Get" parametrelerini sağlayabilir.

```csharp
public class WebQueryConnection : ExternalConnection
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [BackgroundRefresh](../../aspose.cells.externalconnections/externalconnection/backgroundrefresh) { get; set; } | Bağlantının arka planda (eşzamansız olarak) yenilenip yenilenmeyeceğini gösterir. bağlantının tercih edilen kullanımı arka planda zaman uyumsuz olarak yenilemekse true ; false, bağlantının tercih edilen kullanımı ön planda eşzamanlı olarak yenilemekse. |
| [ConnectionDescription](../../aspose.cells.externalconnections/externalconnection/connectiondescription) { get; set; } | Bu bağlantı için kullanıcı tanımını belirtir |
| [ConnectionId](../../aspose.cells.externalconnections/externalconnection/connectionid) { get; } | Bu bağlantının benzersiz tanımlayıcısını belirtir. |
| [CredentialsMethodType](../../aspose.cells.externalconnections/externalconnection/credentialsmethodtype) { get; set; } | Bağlantı kurulurken (veya yeniden kurulurken) kullanılacak kimlik doğrulama yöntemini belirtir. |
| [EditWebPage](../../aspose.cells.externalconnections/webqueryconnection/editwebpage) { get; set; } | Web sorgusu verilerini gösteren, kullanıcıya yönelik web sayfasının URL'si. SourceData="true" ve url'nin bir XML dosyasına başvurmak üzere yeniden yönlendirilmesi durumunda bu URL persisted 'dir. Ardından kullanıcıya yönelik sayfa kullanıcı arayüzünde gösterilebilir ve XML verileri sahne arkasından alınabilir . |
| [HtmlFormat](../../aspose.cells.externalconnections/webqueryconnection/htmlformat) { get; set; } | Web sorgusu verilerini çalışma sayfasına getirirken HTML kaynağından biçimlendirme nasıl yapılır? sourceData True olduğunda geçerlidir. |
| [Id](../../aspose.cells.externalconnections/externalconnection/id) { get; } | Bağlantının kimliğini alır. |
| [IsConsecutive](../../aspose.cells.externalconnections/webqueryconnection/isconsecutive) { get; set; } | Ardışık sınırlayıcıların yalnızca bir sınırlayıcı olarak ele alınması gerekip gerekmediğini belirten işaret. |
| [IsDeleted](../../aspose.cells.externalconnections/externalconnection/isdeleted) { get; set; } | İlişkili çalışma kitabı bağlantısının silinip silinmediğini gösterir. the bağlantısı silinmişse true ; aksi takdirde, false. |
| [IsHtmlTables](../../aspose.cells.externalconnections/webqueryconnection/ishtmltables) { get; set; } | Web sorgularının yalnızca HTML tablolarında çalışıp çalışmayacağını belirten işaret. |
| [IsNew](../../aspose.cells.externalconnections/externalconnection/isnew) { get; set; } | Bağlantı ilk kez yenilenmediyse doğrudur; aksi halde yanlış. Bu durum, kullanıcı, bir sorgunun dönüşü tamamlanmadan önce dosyayı kaydettiğinde ortaya çıkabilir. |
| [IsParsePre](../../aspose.cells.externalconnections/webqueryconnection/isparsepre) { get; set; } | Sayfayı bir sorgu tablosuna içe aktardığınızda, web sayfasındaki HTML PRE etiketlerinde bulunan verilerin sütunlara ayrıştırılıp ayrıştırılmadığını belirten bayrak. |
| [IsSameSettings](../../aspose.cells.externalconnections/webqueryconnection/issamesettings) { get; set; } | İlk satırla aynı genişlik settings ile bir PRE bloğu içindeki tüm tabloların ayrıştırılıp ayrıştırılmayacağını belirten bayrak. |
| [IsTextDates](../../aspose.cells.externalconnections/webqueryconnection/istextdates) { get; set; } | Çalışma sayfasındaki hücrelere tarihlerin tarihler yerine metin olarak içe aktarılması gerekip gerekmediğini belirten işaret. |
| [IsXl2000](../../aspose.cells.externalconnections/webqueryconnection/isxl2000) { get; set; } | Bu işaret, var olan eski elektronik tablo dosyalarıyla geriye dönük uyumluluk için mevcuttur ve bu web sorgusu Microsoft Excel 2000'e eşit veya daha yeni bir elektronik tablo uygulamasında yenilenmişse true olarak ayarlanır. Bu, yoksayılabilecek isteğe bağlı bir özniteliktir. |
| [IsXl97](../../aspose.cells.externalconnections/webqueryconnection/isxl97) { get; set; } | Bu işaret, mevcut eski elektronik tablo dosyalarıyla geriye dönük uyumluluk için mevcuttur ve bu web sorgusu Microsoft Excel 97'de oluşturulmuşsa, true olarak ayarlanır. Bu, yoksayılabilecek isteğe bağlı bir özniteliktir. |
| [IsXml](../../aspose.cells.externalconnections/webqueryconnection/isxml) { get; set; } | web sorgusu kaynağı XML ise (HTML'ye karşı), aksi takdirde false. |
| [IsXmlSourceData](../../aspose.cells.externalconnections/webqueryconnection/isxmlsourcedata) { get; set; } | HTML tablosunun kendisi yerine XML kaynak verilerinin içe aktarılması gerektiğini belirten bayrak. |
| [KeepAlive](../../aspose.cells.externalconnections/externalconnection/keepalive) { get; set; } | Elektronik tablo uygulamasının bağlantısını açık tutmak için çaba göstermesi gerektiğinde doğrudur. Yanlış olduğunda, uygulama bilgilerini aldıktan sonra bağlantıyı kapatmalıdır. |
| [Name](../../aspose.cells.externalconnections/externalconnection/name) { get; set; } | Bağlantının adını belirtir. Her bağlantının benzersiz bir adı olmalıdır. |
| [OdcFile](../../aspose.cells.externalconnections/externalconnection/odcfile) { get; set; } | Bu bağlantının oluşturulduğu harici bağlantı dosyasının tam yolunu belirtir. Verileri yenileme girişimi sırasında bir bağlantı başarısız olursa ve reconnectionMethod=1, ise, elektronik tablo uygulaması, çalışma kitabına katıştırılmış bağlantı nesnesi yerine harici bağlantı dosyasındaki bilgileri kullanmayı tekrar deneyecektir. |
| [OnlyUseConnectionFile](../../aspose.cells.externalconnections/externalconnection/onlyuseconnectionfile) { get; set; } | Elektronik tablo uygulamasının, bağlantı yenilendiğinde odcFile özniteliği tarafından belirtilen harici bağlantı dosyasındaki bağlantı bilgilerini her zaman ve yalnızca kullanması gerekip gerekmediğini gösterir. Yanlışsa, elektronik tablo uygulaması , reconnectionMethod özniteliği tarafından belirtilen prosedürü izlemelidir. |
| [Parameters](../../aspose.cells.externalconnections/externalconnection/parameters) { get; } | Alır[`ConnectionParameterCollection`](../connectionparametercollection) bir ODBC veya web sorgusu için. |
| [Post](../../aspose.cells.externalconnections/webqueryconnection/post) { get; set; } | Bir web sorgusundan veri döndürmek için bir web sunucusuna veri girme post yöntemiyle kullanılan dizeyi döndürür veya ayarlar . |
| virtual [PowerQueryFormula](../../aspose.cells.externalconnections/externalconnection/powerqueryformula) { get; } | Güçlü sorgu formülünün tanımını alır. |
| [ReconnectionMethodType](../../aspose.cells.externalconnections/externalconnection/reconnectionmethodtype) { get; set; } | Bir bağlantı başarısız olduğunda elektronik tablo uygulamasının ne yapması gerektiğini belirtir. Varsayılan değer, ReConnectionMethodType.Required. 'dir. |
| [RefreshInternal](../../aspose.cells.externalconnections/externalconnection/refreshinternal) { get; set; } | Bağlantının otomatik olarak yenilenmesi arasındaki dakika sayısını belirtir. |
| [RefreshOnLoad](../../aspose.cells.externalconnections/externalconnection/refreshonload) { get; set; } | Dosya açılırken bu bağlantının yenilenmesi gerekiyorsa doğrudur; aksi takdirde, false. |
| [SaveData](../../aspose.cells.externalconnections/externalconnection/savedata) { get; set; } | Bir tabloyu doldurmak için bağlantı üzerinden alınan dış veriler çalışma kitabıyla birlikte kaydedilecekse doğrudur; aksi halde yanlış. |
| [SavePassword](../../aspose.cells.externalconnections/externalconnection/savepassword) { get; set; } | Parola bağlantı dizesinin bir parçası olarak kaydedilecekse doğru; aksi takdirde, False. |
| [SourceFile](../../aspose.cells.externalconnections/externalconnection/sourcefile) { get; set; } | Harici veri kaynağı dosya tabanlı olduğunda kullanılır. Böyle bir veri kaynağına bağlantı başarısız olduğunda, elektronik tablo uygulaması doğrudan bu dosyaya bağlanmayı dener. URI veya sisteme özgü dosya yolu gösteriminde ifade edilebilir. |
| [SSOId](../../aspose.cells.externalconnections/externalconnection/ssoid) { get; set; } | Ara elektronik tabloML sunucusu ile harici veri kaynağı arasında kimlik doğrulaması için kullanılan Tekli Oturum Açma (SSO) tanımlayıcısı. |
| [Type](../../aspose.cells.externalconnections/externalconnection/type) { get; set; } | Harici bağlantı DataSource türünü alır veya ayarlar. |
| [Url](../../aspose.cells.externalconnections/webqueryconnection/url) { get; set; } | Harici verileri yenilemek için kullanılacak URL. |

### Ayrıca bakınız

* class [ExternalConnection](../externalconnection)
* ad alanı [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections)
* toplantı [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
