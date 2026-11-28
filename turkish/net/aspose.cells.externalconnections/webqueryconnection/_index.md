---
title: "Sınıf WebQueryConnection"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.ExternalConnections.WebQueryConnection sınıfı. Web sorgu kaynağı için özellikleri belirtir. Bir web sorgusu, HTML tablolarından veri alır ve ayrıca parametreleri ve parametre öğelerini dahil ederek HTML oluşturulurken web sunucusu tarafından işlenmek üzere HTTP Get parametreleri sağlayabilir."
type: docs
url: /tr/net/aspose.cells.externalconnections/webqueryconnection/
---
## WebQueryConnection class

Web sorgu kaynağı için özellikleri belirtir. Bir web sorgusu, HTML tablolarından veri alır ve ayrıca parametreleri ve parametre öğelerini dahil ederek HTML oluşturulurken web sunucusu tarafından işlenmek üzere HTTP \"Get\" parametreleri sağlayabilir.

```csharp
public class WebQueryConnection : ExternalConnection
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [BackgroundRefresh](../../aspose.cells.externalconnections/externalconnection/backgroundrefresh/) { get; set; } | Bağlantının arka planda (asenkron) yenilenip yenilenemeyeceğini gösterir. Bağlantının tercih edilen kullanımı arka planda asenkron yenileme ise true; ön planda senkron yenileme ise false. ([`ExternalConnection`](../externalconnection/) sınıfından devralınmıştır.) |
| override [ClassType](../../aspose.cells.externalconnections/webqueryconnection/classtype/) { get; } | Bu [`ExternalConnection`](../externalconnection/) nesnesinin türünü alır. |
| virtual [Command](../../aspose.cells.externalconnections/externalconnection/command/) { get; set; } | Veritabanı komutunu içeren dize, harici kaynağa etkileşimde bulunmak için veri sağlayıcı API'sine geçirilir ([`ExternalConnection`](../externalconnection/) sınıfından devralınmıştır). |
| virtual [CommandType](../../aspose.cells.externalconnections/externalconnection/commandtype/) { get; set; } | OLE DB komut türünü belirtir. 1. Sorgu bir küp adını belirtir 2. Sorgu bir SQL ifadesini belirtir 3. Sorgu bir tablo adını belirtir 4. Sorgu varsayılan bilginin verildiğini ve yorumlamanın sağlayıcıya bırakıldığını belirtir. 5. Sorgu web tabanlı Liste Veri Sağlayıcısına yöneliktir. ([`ExternalConnection`](../externalconnection/) sınıfından devralınmıştır). |
| [ConnectionDescription](../../aspose.cells.externalconnections/externalconnection/connectiondescription/) { get; set; } | Bu bağlantı için kullanıcı açıklamasını belirtir ([`ExternalConnection`](../externalconnection/) sınıfından devralınmıştır). |
| override [ConnectionFile](../../aspose.cells.externalconnections/webqueryconnection/connectionfile/) { get; } | Bağlantı dosyasını alır. |
| [ConnectionId](../../aspose.cells.externalconnections/externalconnection/connectionid/) { get; } | (**Obsolete.**) Bu bağlantının benzersiz tanımlayıcısını belirtir. ([`ExternalConnection`](../externalconnection/) sınıfından devralınmıştır.) |
| virtual [ConnectionString](../../aspose.cells.externalconnections/externalconnection/connectionstring/) { get; set; } | Bağlantı bilgi dizesi, bir OLE DB veya ODBC veri kaynağıyla iletişim kurmak için kullanılır ([`ExternalConnection`](../externalconnection/) sınıfından devralınmıştır). |
| [Credentials](../../aspose.cells.externalconnections/externalconnection/credentials/) { get; set; } | (**Obsolete.**) Bağlantıyı (yeniden) kurarken kullanılacak kimlik doğrulama yöntemini belirtir. ([`ExternalConnection`](../externalconnection/) sınıfından devralınmıştır.) |
| [CredentialsMethodType](../../aspose.cells.externalconnections/externalconnection/credentialsmethodtype/) { get; set; } | Bağlantıyı (yeniden) kurarken kullanılacak kimlik doğrulama yöntemini belirtir. ([`ExternalConnection`](../externalconnection/) sınıfından devralınmıştır.) |
| [EditPage](../../aspose.cells.externalconnections/webqueryconnection/editpage/) { get; set; } | (**Eski.**) Web sorgu verilerini gösteren kullanıcıya yönelik web sayfasının URL'si. sourceData="true" olduğu ve url'nin bir XML dosyasına yönlendirildiği durumda bu URL korunur. Böylece kullanıcıya yönelik sayfa UI'da gösterilebilir ve XML verisi arka planda alınabilir. |
| [EditWebPage](../../aspose.cells.externalconnections/webqueryconnection/editwebpage/) { get; set; } | Web sorgu verilerini gösteren kullanıcıya yönelik web sayfasının URL'si. sourceData="true" olduğu ve url'nin bir XML dosyasına yönlendirildiği durumda bu URL korunur. Böylece kullanıcıya yönelik sayfa UI'da gösterilebilir ve XML verisi arka planda alınabilir. |
| [HtmlFormat](../../aspose.cells.externalconnections/webqueryconnection/htmlformat/) { get; set; } | HTML kaynağından gelen biçimlendirmeyi, web sorgu verileri çalışma sayfasına getirildiğinde nasıl ele alacağınız. sourceData True olduğunda geçerlidir. |
| [Id](../../aspose.cells.externalconnections/externalconnection/id/) { get; } | Bağlantının kimliğini alır. ([`ExternalConnection`](../externalconnection/) sınıfından devralınmıştır.) |
| [IsConsecutive](../../aspose.cells.externalconnections/webqueryconnection/isconsecutive/) { get; set; } | Ardışık ayırıcıların tek bir ayırıcı olarak ele alınması gerektiğini gösteren işaret. |
| [IsDeleted](../../aspose.cells.externalconnections/externalconnection/isdeleted/) { get; set; } | İlgili çalışma kitabı bağlantısının silinip silinmediğini gösterir. Bağlantı silinmişse true; aksi takdirde false. ([`ExternalConnection`](../externalconnection/) sınıfından devralınmıştır.) |
| [IsHtmlTables](../../aspose.cells.externalconnections/webqueryconnection/ishtmltables/) { get; set; } | Web sorgularının yalnızca HTML tablolarında çalışması gerektiğini gösteren işaret. |
| [IsNew](../../aspose.cells.externalconnections/externalconnection/isnew/) { get; set; } | Bağlantı ilk kez yenilenmemişse true; aksi takdirde false. Bu durum, kullanıcının sorgu tamamlanmadan dosyayı kaydetmesi durumunda ortaya çıkabilir. ([`ExternalConnection`](../externalconnection/) sınıfından devralınmıştır.) |
| [IsParsePre](../../aspose.cells.externalconnections/webqueryconnection/isparsepre/) { get; set; } | Web sayfasındaki HTML PRE etiketleri içinde bulunan verilerin, sayfa bir sorgu tablosuna içe aktarıldığında sütunlara ayrılıp ayrılmayacağını gösteren işaret. |
| [IsSameSettings](../../aspose.cells.externalconnections/webqueryconnection/issamesettings/) { get; set; } | İlk satırın aynı genişlik ayarlarıyla PRE bloğu içindeki tüm tabloların ayrılıp ayrılmayacağını gösteren işaret. |
| [IsTextDates](../../aspose.cells.externalconnections/webqueryconnection/istextdates/) { get; set; } | Tarihlerin, çalışma sayfasındaki hücrelere tarih olarak değil metin olarak aktarılması gerektiğini gösteren işaret. |
| [IsXl2000](../../aspose.cells.externalconnections/webqueryconnection/isxl2000/) { get; set; } | Bu bayrak, daha eski mevcut elektronik tablo dosyalarıyla geriye dönük uyumluluk sağlamak için bulunur ve bu web sorgusu Microsoft Excel 2000 veya daha yeni bir elektronik tablo uygulamasında yenilendiğinde true olarak ayarlanır. Bu, göz ardı edilebilecek isteğe bağlı bir özelliktir. |
| [IsXl97](../../aspose.cells.externalconnections/webqueryconnection/isxl97/) { get; set; } | Bu bayrak, daha eski mevcut elektronik tablo dosyalarıyla geriye dönük uyumluluk sağlamak için bulunur ve bu web sorgusu Microsoft Excel 97'de oluşturulduğunda true olarak ayarlanır. Bu, göz ardı edilebilecek isteğe bağlı bir özelliktir. |
| [IsXml](../../aspose.cells.externalconnections/webqueryconnection/isxml/) { get; set; } | web sorgu kaynağı XML ise true, aksi takdirde false. |
| [IsXmlSourceData](../../aspose.cells.externalconnections/webqueryconnection/isxmlsourcedata/) { get; set; } | HTML tablosu yerine XML kaynak verisinin içe aktarılması gerektiğini gösteren bayrak. |
| [KeepAlive](../../aspose.cells.externalconnections/externalconnection/keepalive/) { get; set; } | E-tablo uygulaması bağlantıyı açık tutmak için çaba göstermeli ise true. False olduğunda, uygulama bilgiyi aldıktan sonra bağlantıyı kapatmalıdır. ([`ExternalConnection`](../externalconnection/) sınıfından devralınmıştır.) |
| [Name](../../aspose.cells.externalconnections/externalconnection/name/) { get; set; } | Bağlantının adını belirtir. Her bağlantının benzersiz bir adı olmalıdır. ([`ExternalConnection`](../externalconnection/) sınıfından devralınmıştır.) |
| [OdcFile](../../aspose.cells.externalconnections/externalconnection/odcfile/) { get; set; } | Bu bağlantının oluşturulduğu dış bağlantı dosyasının tam yolunu belirtir. Veri yenileme girişimi sırasında bir bağlantı başarısız olursa ve reconnectionMethod=1 ise, elektronik tablo uygulaması, çalışma kitabına gömülü bağlantı nesnesi yerine dış bağlantı dosyasındaki bilgileri kullanarak tekrar deneyecektir. ([`ExternalConnection`](../externalconnection/) sınıfından devralınmıştır.) |
| [OnlyUseConnectionFile](../../aspose.cells.externalconnections/externalconnection/onlyuseconnectionfile/) { get; set; } | Bağlantı yenilendiğinde elektronik tablo uygulamasının, odcFile özniteliğiyle belirtilen dış bağlantı dosyasındaki bağlantı bilgilerini her zaman ve yalnızca kullanıp kullanmayacağını gösterir. Yanlış ise, elektronik tablo uygulaması reconnectionMethod özniteliğiyle belirtilen prosedürü izlemelidir. ([`ExternalConnection`](../externalconnection/) sınıfından devralınmıştır.) |
| [Parameters](../../aspose.cells.externalconnections/externalconnection/parameters/) { get; } | ODBC veya web sorgusu için [`ConnectionParameterCollection`](../connectionparametercollection/) alır. ([`ExternalConnection`](../externalconnection/) sınıfından devralınmıştır.) |
| [Post](../../aspose.cells.externalconnections/webqueryconnection/post/) { get; set; } | Bir web sorgusundan veri döndürmek için verileri bir web sunucusuna gönderirken kullanılan post yöntemiyle kullanılan dizeyi alır veya ayarlar. |
| virtual [PowerQueryFormula](../../aspose.cells.externalconnections/externalconnection/powerqueryformula/) { get; } | Power query formülünün tanımını alır. ([`ExternalConnection`](../externalconnection/) sınıfından devralınmıştır.) |
| [ReconnectionMethod](../../aspose.cells.externalconnections/externalconnection/reconnectionmethod/) { get; set; } | (**Obsolete.**) Bir bağlantı başarısız olduğunda elektronik tablo uygulamasının ne yapması gerektiğini belirtir. Varsayılan değer ReConnectionMethodType.Required'dir. ([`ExternalConnection`](../externalconnection/) sınıfından devralınmıştır.) |
| [ReconnectionMethodType](../../aspose.cells.externalconnections/externalconnection/reconnectionmethodtype/) { get; set; } | Bir bağlantı başarısız olduğunda elektronik tablo uygulamasının ne yapması gerektiğini belirtir. Varsayılan değer ReConnectionMethodType.Required'dir. ([`ExternalConnection`](../externalconnection/) sınıfından devralınmıştır.) |
| [RefreshInternal](../../aspose.cells.externalconnections/externalconnection/refreshinternal/) { get; set; } | Bağlantının otomatik yenilemeleri arasındaki dakika sayısını belirtir. ([`ExternalConnection`](../externalconnection/) sınıfından devralınmıştır.) |
| [RefreshOnLoad](../../aspose.cells.externalconnections/externalconnection/refreshonload/) { get; set; } | Dosya açıldığında bu bağlantının yenilenmesi gerekiyorsa doğru; aksi takdirde yanlış. ([`ExternalConnection`](../externalconnection/) sınıfından devralınmıştır.) |
| [SaveData](../../aspose.cells.externalconnections/externalconnection/savedata/) { get; set; } | Bağlantı üzerinden alınan dış verinin bir tabloyu doldurmak için çalışma kitabıyla birlikte kaydedilmesi gerekiyorsa doğru; aksi takdirde yanlış. ([`ExternalConnection`](../externalconnection/) sınıfından devralınmıştır.) |
| [SavePassword](../../aspose.cells.externalconnections/externalconnection/savepassword/) { get; set; } | Parolanın bağlantı dizesinin bir parçası olarak kaydedilmesi gerekiyorsa doğru; aksi takdirde Yanlış. ([`ExternalConnection`](../externalconnection/) sınıfından devralınmıştır.) |
| virtual [SecondCommand](../../aspose.cells.externalconnections/externalconnection/secondcommand/) { get; set; } | PivotTable sunucu tabanlı sayfa alanları kullanıldığında kalıcı olan ikinci komut metni dizesini belirtir. ODBC bağlantıları için serverCommand genellikle komuttan daha geniş bir sorgudur (ilkinde WHERE koşulu yoktur). Bu 2 komuta (Command ve ServerCommand) dayanarak, parametre UI'si doldurulabilir ve parametreli sorgular oluşturulabilir ([`ExternalConnection`](../externalconnection/) üzerinden devralınmıştır). |
| [SourceFile](../../aspose.cells.externalconnections/externalconnection/sourcefile/) { get; set; } | Dış veri kaynağı dosya tabanlı olduğunda kullanılır. Böyle bir veri kaynağına bağlantı başarısız olduğunda, elektronik tablo uygulaması bu dosyaya doğrudan bağlanmaya çalışır. URI veya sistem‑özgü dosya yolu gösterimiyle ifade edilebilir. ([`ExternalConnection`](../externalconnection/) sınıfından devralınmıştır.) |
| [SourceType](../../aspose.cells.externalconnections/externalconnection/sourcetype/) { get; set; } | Dış bağlantı DataSource türünü alır veya ayarlar. ([`ExternalConnection`](../externalconnection/) sınıfından devralınmıştır.) |
| [SSOId](../../aspose.cells.externalconnections/externalconnection/ssoid/) { get; set; } | Ara bir spreadsheetML sunucusu ile dış veri kaynağı arasındaki kimlik doğrulama için kullanılan Tek Oturum Açma (SSO) tanımlayıcısı. ([`ExternalConnection`](../externalconnection/) sınıfından devralınmıştır.) |
| [Type](../../aspose.cells.externalconnections/externalconnection/type/) { get; set; } | (**Obsolete.**) Dış bağlantı DataSource türünü alır veya ayarlar. ([`ExternalConnection`](../externalconnection/) sınıfından devralınmıştır.) |
| [Url](../../aspose.cells.externalconnections/webqueryconnection/url/) { get; set; } | Harici verileri yenilemek için kullanılacak URL. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionsClassWebQueryConnectionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();

            try
            {
                // Koleksiyon aracılığıyla web sorgu bağlantısı oluştur
                WebQueryConnection connection = (WebQueryConnection)workbook.DataConnections[workbook.DataConnections.Count];
                
                connection.Url = "https://example.com/financial-data";
                connection.IsHtmlTables = true;
                connection.IsTextDates = true;
                connection.HtmlFormat = HtmlFormatHandlingType.All;

                Console.WriteLine($"Web query URL: {connection.Url}");
                Console.WriteLine($"HTML tables only: {connection.IsHtmlTables}");

                workbook.Save("WebQueryConnectionDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with WebQueryConnection: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [ExternalConnection](../externalconnection/)
* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


