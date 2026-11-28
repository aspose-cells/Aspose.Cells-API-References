---
title: "Sınıf ExternalConnection"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.ExternalConnections.ExternalConnection sınıfı. Harici bir veri bağlantısını belirtir"
type: docs
url: /tr/net/aspose.cells.externalconnections/externalconnection/
---
## ExternalConnection class

Harici bir veri bağlantısını belirtir

```csharp
public abstract class ExternalConnection
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [BackgroundRefresh](../../aspose.cells.externalconnections/externalconnection/backgroundrefresh/) { get; set; } | Bağlantının arka planda (eşzamansız) yenilenip yenilenemeyeceğini gösterir. Bağlantının tercih edilen kullanımının arka planda eşzamansız olarak yenilenmesi ise true; ön planda senkron olarak yenilenmesi ise false. |
| abstract [ClassType](../../aspose.cells.externalconnections/externalconnection/classtype/) { get; } | `ExternalConnection` nesnesinin türünü alır. |
| virtual [Command](../../aspose.cells.externalconnections/externalconnection/command/) { get; set; } | Veri sağlayıcı API'sine dış kaynağa etkileşimde bulunarak veri almak için gönderilecek veritabanı komutunu içeren dize. |
| virtual [CommandType](../../aspose.cells.externalconnections/externalconnection/commandtype/) { get; set; } | OLE DB komut türünü belirtir. 1. Sorgu bir küp adını belirtir 2. Sorgu bir SQL ifadesi belirtir 3. Sorgu bir tablo adını belirtir 4. Sorgu varsayılan bilgilerin verildiğini belirtir ve yorumlama sağlayıcıya bırakılır 5. Sorgu web tabanlı List Data Provider'a yöneliktir. |
| [ConnectionDescription](../../aspose.cells.externalconnections/externalconnection/connectiondescription/) { get; set; } | Bu bağlantı için kullanıcı açıklamasını belirtir. |
| virtual [ConnectionFile](../../aspose.cells.externalconnections/externalconnection/connectionfile/) { get; } | Bağlantı dosyasını alır. |
| [ConnectionId](../../aspose.cells.externalconnections/externalconnection/connectionid/) { get; } | (**Obsolete.**) Bu bağlantının benzersiz tanımlayıcısını belirtir. |
| virtual [ConnectionString](../../aspose.cells.externalconnections/externalconnection/connectionstring/) { get; set; } | Bağlantı bilgi dizesi, bir OLE DB veya ODBC veri kaynağıyla iletişim kurmak için kullanılır. |
| [Credentials](../../aspose.cells.externalconnections/externalconnection/credentials/) { get; set; } | (**Obsolete.**) Bağlantıyı kurarken (veya yeniden kurarken) kullanılacak kimlik doğrulama yöntemini belirtir. |
| [CredentialsMethodType](../../aspose.cells.externalconnections/externalconnection/credentialsmethodtype/) { get; set; } | Bağlantıyı kurarken (veya yeniden kurarken) kullanılacak kimlik doğrulama yöntemini belirtir. |
| [Id](../../aspose.cells.externalconnections/externalconnection/id/) { get; } | Bağlantının kimliğini alır. |
| [IsDeleted](../../aspose.cells.externalconnections/externalconnection/isdeleted/) { get; set; } | İlgili çalışma kitabı bağlantısının silinip silinmediğini gösterir. Bağlantı silinmişse true; aksi takdirde false. |
| [IsNew](../../aspose.cells.externalconnections/externalconnection/isnew/) { get; set; } | Bağlantı ilk kez yenilenmemişse true; aksi takdirde false. Bu durum, kullanıcının sorgu tamamlanmadan dosyayı kaydetmesi durumunda ortaya çıkabilir. |
| [KeepAlive](../../aspose.cells.externalconnections/externalconnection/keepalive/) { get; set; } | Bağlantının açık tutulması için elektronik tablo uygulamasının çaba göstermesi gerektiğinde true. False olduğunda, uygulama bilgiyi aldıktan sonra bağlantıyı kapatmalıdır. |
| [Name](../../aspose.cells.externalconnections/externalconnection/name/) { get; set; } | Bağlantının adını belirtir. Her bağlantının benzersiz bir adı olmalıdır. |
| [OdcFile](../../aspose.cells.externalconnections/externalconnection/odcfile/) { get; set; } | Bu bağlantının oluşturulduğu harici bağlantı dosyasının tam yolunu belirtir. Veri yenileme girişimi sırasında bir bağlantı başarısız olur ve reconnectionMethod=1 ise, elektronik tablo uygulaması, çalışma kitabına gömülü bağlantı nesnesi yerine harici bağlantı dosyasındaki bilgileri kullanarak yeniden deneyecektir. |
| [OnlyUseConnectionFile](../../aspose.cells.externalconnections/externalconnection/onlyuseconnectionfile/) { get; set; } | Bağlantı yenilendiğinde elektronik tablo uygulamasının, odcFile özniteliğiyle belirtilen harici bağlantı dosyasındaki bağlantı bilgilerini her zaman ve yalnızca kullanıp kullanmayacağını gösterir. False ise, uygulama reconnectionMethod özniteliğiyle belirtilen prosedürü izlemelidir. |
| [Parameters](../../aspose.cells.externalconnections/externalconnection/parameters/) { get; } | ODBC veya web sorgusu için [`ConnectionParameterCollection`](../connectionparametercollection/) alır. |
| virtual [PowerQueryFormula](../../aspose.cells.externalconnections/externalconnection/powerqueryformula/) { get; } | Power query formülünün tanımını alır. |
| [ReconnectionMethod](../../aspose.cells.externalconnections/externalconnection/reconnectionmethod/) { get; set; } | (**Obsolete.**) Bir bağlantı başarısız olduğunda elektronik tablo uygulamasının ne yapması gerektiğini belirtir. Varsayılan değer ReConnectionMethodType.Required. |
| [ReconnectionMethodType](../../aspose.cells.externalconnections/externalconnection/reconnectionmethodtype/) { get; set; } | Bir bağlantı başarısız olduğunda elektronik tablo uygulamasının ne yapması gerektiğini belirtir. Varsayılan değer ReConnectionMethodType.Required. |
| [RefreshInternal](../../aspose.cells.externalconnections/externalconnection/refreshinternal/) { get; set; } | Bağlantının otomatik yenilemeleri arasındaki dakika sayısını belirtir. |
| [RefreshOnLoad](../../aspose.cells.externalconnections/externalconnection/refreshonload/) { get; set; } | Dosya açıldığında bu bağlantının yenilenmesi gerekiyorsa doğru; aksi takdirde yanlış. |
| [SaveData](../../aspose.cells.externalconnections/externalconnection/savedata/) { get; set; } | Bağlantı üzerinden alınan ve bir tabloyu doldurmak için kullanılan harici veriler çalışma kitabı ile birlikte kaydedilecekse doğru; aksi takdirde yanlış. |
| [SavePassword](../../aspose.cells.externalconnections/externalconnection/savepassword/) { get; set; } | Parola bağlantı dizesinin bir parçası olarak kaydedilecekse doğru; aksi takdirde Yanlış. |
| virtual [SecondCommand](../../aspose.cells.externalconnections/externalconnection/secondcommand/) { get; set; } | PivotTable sunucu tabanlı sayfa alanları kullanıldığında kalıcı olan ikinci komut metin dizesini belirtir. ODBC bağlantıları için serverCommand genellikle command'tan daha geniş bir sorgudur (ilkinde WHERE koşulu bulunmaz). Bu iki komuta (Command ve ServerCommand) dayanarak, parametre UI'si doldurulabilir ve parametreli sorgular oluşturulabilir. |
| [SourceFile](../../aspose.cells.externalconnections/externalconnection/sourcefile/) { get; set; } | Harici veri kaynağı dosya tabanlı olduğunda kullanılır. Böyle bir veri kaynağına bağlantı başarısız olduğunda, elektronik tablo uygulaması doğrudan bu dosyaya bağlanmayı dener. URI veya sistem‑özel dosya yolu gösterimiyle ifade edilebilir. |
| [SourceType](../../aspose.cells.externalconnections/externalconnection/sourcetype/) { get; set; } | Harici bağlantının DataSource türünü alır veya ayarlar. |
| [SSOId](../../aspose.cells.externalconnections/externalconnection/ssoid/) { get; set; } | Ara bir spreadsheetML sunucusu ile harici veri kaynağı arasında kimlik doğrulama için kullanılan Tek Oturum Açma (SSO) tanımlayıcısı. |
| [Type](../../aspose.cells.externalconnections/externalconnection/type/) { get; set; } | (**Eski.**) Harici bağlantının DataSource türünü alır veya ayarlar. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class ExternalConnectionsClassExternalConnectionDemo
    {
        public static void Run()
        {
            string sourceDir = "Your Source Directory";

            Workbook workbook = new Workbook(sourceDir + "example.xlsx");
            ExternalConnectionCollection conns = workbook.DataConnections;
            foreach (ExternalConnection conn in conns)
            {
                if (conn is DBConnection dbConn)
                {
                    Console.WriteLine("Connection Info: " + dbConn.ConnectionInfo);
                    Console.WriteLine("Formula Definition: " + dbConn.PowerQueryFormula.FormulaDefinition);
                }
            }

            workbook = new Workbook(sourceDir + "example.xlsm");
            conns = workbook.DataConnections;
            foreach (ExternalConnection conn in conns)
            {
                if (conn is DBConnection dbConn)
                {
                    Console.WriteLine("Connection Info: " + dbConn.ConnectionInfo);
                    Console.WriteLine("Formula Definition: " + dbConn.PowerQueryFormula.FormulaDefinition);
                }
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


