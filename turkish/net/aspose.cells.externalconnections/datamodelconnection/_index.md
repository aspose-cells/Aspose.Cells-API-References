---
title: "Sınıf DataModelConnection"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.ExternalConnections.DataModelConnection sınıfı. Bir veri modeli bağlantısını belirtir."
type: docs
url: /tr/net/aspose.cells.externalconnections/datamodelconnection/
---
## DataModelConnection class

Bir veri modeli bağlantısını belirtir

```csharp
public class DataModelConnection : ExternalConnection
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [BackgroundRefresh](../../aspose.cells.externalconnections/externalconnection/backgroundrefresh/) { get; set; } | Bağlantının arka planda (asenkron) yenilenip yenilenemeyeceğini gösterir. Bağlantının tercih edilen kullanımı arka planda asenkron yenileme ise true; ön planda senkron yenileme ise false. ([`ExternalConnection`](../externalconnection/) sınıfından devralınmıştır.) |
| override [ClassType](../../aspose.cells.externalconnections/datamodelconnection/classtype/) { get; } | Bu [`ExternalConnection`](../externalconnection/) nesnesinin türünü alır. |
| override [Command](../../aspose.cells.externalconnections/datamodelconnection/command/) { get; set; } | Veri sağlayıcı API'sine dış kaynağa etkileşimde bulunarak veri almak için gönderilecek veritabanı komutunu içeren dize. |
| override [CommandType](../../aspose.cells.externalconnections/datamodelconnection/commandtype/) { get; set; } | [`OLEDBCommandType`](../oledbcommandtype/) tipini döndürür. |
| [ConnectionDescription](../../aspose.cells.externalconnections/externalconnection/connectiondescription/) { get; set; } | Bu bağlantı için kullanıcı açıklamasını belirtir ([`ExternalConnection`](../externalconnection/) sınıfından devralınmıştır). |
| virtual [ConnectionFile](../../aspose.cells.externalconnections/externalconnection/connectionfile/) { get; } | Bağlantı dosyasını alır. ([`ExternalConnection`](../externalconnection/) sınıfından devralınmıştır.) |
| [ConnectionId](../../aspose.cells.externalconnections/externalconnection/connectionid/) { get; } | (**Obsolete.**) Bu bağlantının benzersiz tanımlayıcısını belirtir. ([`ExternalConnection`](../externalconnection/) sınıfından devralınmıştır.) |
| override [ConnectionString](../../aspose.cells.externalconnections/datamodelconnection/connectionstring/) { get; set; } | Bağlantı bilgi dizesi, bir OLE DB veya ODBC veri kaynağıyla iletişim kurmak için kullanılır. |
| [Credentials](../../aspose.cells.externalconnections/externalconnection/credentials/) { get; set; } | (**Obsolete.**) Bağlantıyı (yeniden) kurarken kullanılacak kimlik doğrulama yöntemini belirtir. ([`ExternalConnection`](../externalconnection/) sınıfından devralınmıştır.) |
| [CredentialsMethodType](../../aspose.cells.externalconnections/externalconnection/credentialsmethodtype/) { get; set; } | Bağlantıyı (yeniden) kurarken kullanılacak kimlik doğrulama yöntemini belirtir. ([`ExternalConnection`](../externalconnection/) sınıfından devralınmıştır.) |
| [Id](../../aspose.cells.externalconnections/externalconnection/id/) { get; } | Bağlantının kimliğini alır. ([`ExternalConnection`](../externalconnection/) sınıfından devralınmıştır.) |
| [IsDeleted](../../aspose.cells.externalconnections/externalconnection/isdeleted/) { get; set; } | İlgili çalışma kitabı bağlantısının silinip silinmediğini gösterir. Bağlantı silinmişse true; aksi takdirde false. ([`ExternalConnection`](../externalconnection/) sınıfından devralınmıştır.) |
| [IsNew](../../aspose.cells.externalconnections/externalconnection/isnew/) { get; set; } | Bağlantı ilk kez yenilenmemişse true; aksi takdirde false. Bu durum, kullanıcının sorgu tamamlanmadan dosyayı kaydetmesi durumunda ortaya çıkabilir. ([`ExternalConnection`](../externalconnection/) sınıfından devralınmıştır.) |
| [KeepAlive](../../aspose.cells.externalconnections/externalconnection/keepalive/) { get; set; } | E-tablo uygulaması bağlantıyı açık tutmak için çaba göstermeli ise true. False olduğunda, uygulama bilgiyi aldıktan sonra bağlantıyı kapatmalıdır. ([`ExternalConnection`](../externalconnection/) sınıfından devralınmıştır.) |
| [Name](../../aspose.cells.externalconnections/externalconnection/name/) { get; set; } | Bağlantının adını belirtir. Her bağlantının benzersiz bir adı olmalıdır. ([`ExternalConnection`](../externalconnection/) sınıfından devralınmıştır.) |
| [OdcFile](../../aspose.cells.externalconnections/externalconnection/odcfile/) { get; set; } | Bu bağlantının oluşturulduğu dış bağlantı dosyasının tam yolunu belirtir. Veri yenileme girişimi sırasında bir bağlantı başarısız olursa ve reconnectionMethod=1 ise, elektronik tablo uygulaması, çalışma kitabına gömülü bağlantı nesnesi yerine dış bağlantı dosyasındaki bilgileri kullanarak tekrar deneyecektir. ([`ExternalConnection`](../externalconnection/) sınıfından devralınmıştır.) |
| [OnlyUseConnectionFile](../../aspose.cells.externalconnections/externalconnection/onlyuseconnectionfile/) { get; set; } | Bağlantı yenilendiğinde elektronik tablo uygulamasının, odcFile özniteliğiyle belirtilen dış bağlantı dosyasındaki bağlantı bilgilerini her zaman ve yalnızca kullanıp kullanmayacağını gösterir. Yanlış ise, elektronik tablo uygulaması reconnectionMethod özniteliğiyle belirtilen prosedürü izlemelidir. ([`ExternalConnection`](../externalconnection/) sınıfından devralınmıştır.) |
| [Parameters](../../aspose.cells.externalconnections/externalconnection/parameters/) { get; } | ODBC veya web sorgusu için [`ConnectionParameterCollection`](../connectionparametercollection/) alır. ([`ExternalConnection`](../externalconnection/) sınıfından devralınmıştır.) |
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

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;
    using System.Collections.Generic;

    public class ExternalConnectionsClassDataModelConnectionDemo
    {
        public static void Run()
        {
            // Demonstrasyon için yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            try
            {
                // Yansıma kullanarak DataModelConnection sınıfının bir örneğini oluşturun
                DataModelConnection connection = (DataModelConnection)System.Runtime.Serialization.FormatterServices.GetUninitializedObject(typeof(DataModelConnection));

                // Temel özellikleri ayarlayın
                connection.Command = "SELECT * FROM Products";
                connection.CommandType = OLEDBCommandType.SqlStatement;
                connection.ConnectionString = "Provider=SQLOLEDB;Data Source=Northwind;Integrated Security=SSPI";

                // Bağlantıyı çalışma kitabının veri bağlantılarına ekleyin
                ((IList<ExternalConnection>)workbook.DataConnections).Add(connection);

                // Bağlantı bilgilerini görüntüleyin
                Console.WriteLine($"Connection Type: {connection.ClassType}");
                Console.WriteLine($"Command: {connection.Command}");
                Console.WriteLine($"Command Type: {connection.CommandType}");
                Console.WriteLine($"Connection String: {connection.ConnectionString}");

                // Çalışma kitabını kaydedin
                workbook.Save("DataModelConnectionDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with DataModelConnection.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with DataModelConnection: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [ExternalConnection](../externalconnection/)
* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


