---
title: "DBConnection Sınıfı"
linktitle: "DBConnection"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "DBConnection sınıfı. Go'da dbconnection'ı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/dbconnection/
---

## DBConnection class

ODBC veya OLE DB harici veri bağlantısıyla ilişkili tüm özellikleri belirtir.

```go

type DBConnection struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewDBConnection](./newdbconnection/) | Bir üst nesneden oluşturur. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetClassType](./getclasstype/) | Bu ExternalConnection nesnesinin türünü alır. |
| [GetConnectionString](./getconnectionstring/) | Bağlantı bilgi dizesi, bir OLE DB veya ODBC veri kaynağıyla iletişim kurmak için kullanılır. |
| [SetConnectionString](./setconnectionstring/) | Bağlantı bilgi dizesi, bir OLE DB veya ODBC veri kaynağıyla iletişim kurmak için kullanılır. |
| [GetPowerQueryFormula](./getpowerqueryformula/) | Power Query formülünün tanımını alır. |
| [GetCommandType](./getcommandtype/) | OLE DB komut türünü belirtir.1. Sorgu bir küp adını belirtir2. Sorgu bir SQL ifadesi belirtir3. Sorgu bir tablo adını belirtir4. Sorgu varsayılan bilgilerin verildiğini belirtir ve yorumlama sağlayıcıya bırakılır.5. Sorgu web tabanlı List Data Provider'a yöneliktir. |
| [SetCommandType](./setcommandtype/) | OLE DB komut türünü belirtir.1. Sorgu bir küp adını belirtir2. Sorgu bir SQL ifadesi belirtir3. Sorgu bir tablo adını belirtir4. Sorgu varsayılan bilgilerin verildiğini belirtir ve yorumlama sağlayıcıya bırakılır.5. Sorgu web tabanlı List Data Provider'a yöneliktir. |
| [GetCommand](./getcommand/) | Harici kaynaktan veri almak için veri sağlayıcı API'sine iletilecek veritabanı komutunu içeren dize. |
| [SetCommand](./setcommand/) | Harici kaynaktan veri almak için veri sağlayıcı API'sine iletilecek veritabanı komutunu içeren dize. |
| [GetSecondCommand](./getsecondcommand/) | PivotTable sunucu tabanlı sayfa alanları kullanıldığında kalıcı olan ikinci bir komut metni dizesini belirtir. ODBC bağlantılarında, serverCommand genellikle command'tan daha geniş bir sorgudur (ilkinde WHERE koşulu yoktur). Bu iki komuta (Command ve ServerCommand) dayanarak, parametre UI'si doldurulabilir ve parametreli sorgular oluşturulabilir. |
| [SetSecondCommand](./setsecondcommand/) | PivotTable sunucu tabanlı sayfa alanları kullanıldığında kalıcı olan ikinci bir komut metni dizesini belirtir. ODBC bağlantılarında, serverCommand genellikle command'tan daha geniş bir sorgudur (ilkinde WHERE koşulu yoktur). Bu iki komuta (Command ve ServerCommand) dayanarak, parametre UI'si doldurulabilir ve parametreli sorgular oluşturulabilir. |
| [GetId](./getid/) | Bağlantının kimliğini alır. |
| [GetSourceType](./getsourcetype/) | Harici bağlantı DataSource türünü alır veya ayarlar. |
| [SetSourceType](./setsourcetype/) | Harici bağlantı DataSource türünü alır veya ayarlar. |
| [GetSSOId](./getssoid/) | Ara sunucu spreadsheetML sunucusu ile harici veri kaynağı arasında kimlik doğrulama için kullanılan Single Sign On (SSO) tanımlayıcısı. |
| [SetSSOId](./setssoid/) | Ara sunucu spreadsheetML sunucusu ile harici veri kaynağı arasında kimlik doğrulama için kullanılan Single Sign On (SSO) tanımlayıcısı. |
| [GetSavePassword](./getsavepassword/) | Parola bağlantı dizesinin bir parçası olarak kaydedilecekse doğru; aksi takdirde Yanlış. |
| [SetSavePassword](./setsavepassword/) | Parola bağlantı dizesinin bir parçası olarak kaydedilecekse doğru; aksi takdirde Yanlış. |
| [GetSaveData](./getsavedata/) | Bağlantı üzerinden alınan ve bir tabloyu doldurmak için kullanılan harici veri çalışma kitabıyla birlikte kaydedilecekse doğru; aksi takdirde yanlış. |
| [SetSaveData](./setsavedata/) | Bağlantı üzerinden alınan ve bir tabloyu doldurmak için kullanılan harici veri çalışma kitabıyla birlikte kaydedilecekse doğru; aksi takdirde yanlış. |
| [GetRefreshOnLoad](./getrefreshonload/) | Dosya açıldığında bu bağlantının yenilenmesi gerekiyorsa doğru; aksi takdirde yanlış. |
| [SetRefreshOnLoad](./setrefreshonload/) | Dosya açıldığında bu bağlantının yenilenmesi gerekiyorsa doğru; aksi takdirde yanlış. |
| [GetReconnectionMethodType](./getreconnectionmethodtype/) | Bir bağlantı başarısız olduğunda elektronik tablo uygulamasının ne yapması gerektiğini belirtir. Varsayılan değer ReConnectionMethodType.Required'tır. |
| [SetReconnectionMethodType](./setreconnectionmethodtype/) | Bir bağlantı başarısız olduğunda elektronik tablo uygulamasının ne yapması gerektiğini belirtir. Varsayılan değer ReConnectionMethodType.Required'tır. |
| [GetOnlyUseConnectionFile](./getonlyuseconnectionfile/) | Bağlantı yenilendiğinde elektronik tablo uygulamasının her zaman ve yalnızca odcFile özniteliğiyle belirtilen harici bağlantı dosyasındaki bağlantı bilgilerini kullanıp kullanmayacağını gösterir. Yanlış ise, elektronik tablo uygulaması reconnectionMethod özniteliğiyle belirtilen prosedürü izlemelidir. |
| [SetOnlyUseConnectionFile](./setonlyuseconnectionfile/) | Bağlantı yenilendiğinde elektronik tablo uygulamasının her zaman ve yalnızca odcFile özniteliğiyle belirtilen harici bağlantı dosyasındaki bağlantı bilgilerini kullanıp kullanmayacağını gösterir. Yanlış ise, elektronik tablo uygulaması reconnectionMethod özniteliğiyle belirtilen prosedürü izlemelidir. |
| [GetOdcFile](./getodcfile/) | Bu bağlantının oluşturulduğu harici bağlantı dosyasının tam yolunu belirtir. Veri yenileme girişimi sırasında bir bağlantı başarısız olur ve reconnectionMethod=1 ise, elektronik tablo uygulaması, çalışma kitabına gömülü bağlantı nesnesi yerine harici bağlantı dosyasındaki bilgileri kullanarak tekrar deneyecektir. |
| [SetOdcFile](./setodcfile/) | Bu bağlantının oluşturulduğu harici bağlantı dosyasının tam yolunu belirtir. Veri yenileme girişimi sırasında bir bağlantı başarısız olur ve reconnectionMethod=1 ise, elektronik tablo uygulaması, çalışma kitabına gömülü bağlantı nesnesi yerine harici bağlantı dosyasındaki bilgileri kullanarak tekrar deneyecektir. |
| [GetSourceFile](./getsourcefile/) | Harici veri kaynağı dosya tabanlı olduğunda kullanılır. Böyle bir veri kaynağına bağlantı başarısız olduğunda, elektronik tablo uygulaması doğrudan bu dosyaya bağlanmayı dener. URI veya sistem‑özel dosya yolu gösterimiyle ifade edilebilir. |
| [SetSourceFile](./setsourcefile/) | Harici veri kaynağı dosya tabanlı olduğunda kullanılır. Böyle bir veri kaynağına bağlantı başarısız olduğunda, elektronik tablo uygulaması doğrudan bu dosyaya bağlanmayı dener. URI veya sistem‑özel dosya yolu gösterimiyle ifade edilebilir. |
| [IsNew](./isnew/) | Bağlantı ilk kez yenilenmemişse doğru; aksi takdirde yanlış. Bu durum, kullanıcının sorgu tamamlanmadan dosyayı kaydetmesi durumunda ortaya çıkabilir. |
| [SetIsNew](./setisnew/) | Bağlantı ilk kez yenilenmemişse doğru; aksi takdirde yanlış. Bu durum, kullanıcının sorgu tamamlanmadan dosyayı kaydetmesi durumunda ortaya çıkabilir. |
| [GetName](./getname/) | Bağlantının adını belirtir. Her bağlantının benzersiz bir adı olmalıdır. |
| [SetName](./setname/) | Bağlantının adını belirtir. Her bağlantının benzersiz bir adı olmalıdır. |
| [GetKeepAlive](./getkeepalive/) | Elektronik tablo uygulamasının bağlantıyı açık tutmak için çaba göstermesi gerekiyorsa doğru. Yanlış ise, uygulama bilgiyi aldıktan sonra bağlantıyı kapatmalıdır. |
| [SetKeepAlive](./setkeepalive/) | Elektronik tablo uygulamasının bağlantıyı açık tutmak için çaba göstermesi gerekiyorsa doğru. Yanlış ise, uygulama bilgiyi aldıktan sonra bağlantıyı kapatmalıdır. |
| [GetRefreshInternal](./getrefreshinternal/) | Bağlantının otomatik yenilenmeleri arasındaki dakika sayısını belirtir. |
| [SetRefreshInternal](./setrefreshinternal/) | Bağlantının otomatik yenilenmeleri arasındaki dakika sayısını belirtir. |
| [GetConnectionDescription](./getconnectiondescription/) | Bu bağlantı için kullanıcı açıklamasını belirtir |
| [SetConnectionDescription](./setconnectiondescription/) | Bu bağlantı için kullanıcı açıklamasını belirtir |
| [IsDeleted](./isdeleted/) | İlgili çalışma kitabı bağlantısının silinip silinmediğini gösterir. Bağlantı silinmişse doğru; aksi takdirde yanlış. |
| [SetIsDeleted](./setisdeleted/) | İlgili çalışma kitabı bağlantısının silinip silinmediğini gösterir. Bağlantı silinmişse doğru; aksi takdirde yanlış. |
| [GetCredentialsMethodType](./getcredentialsmethodtype/) | Bağlantıyı (veya yeniden bağlanmayı) kurarken kullanılacak kimlik doğrulama yöntemini belirtir. |
| [SetCredentialsMethodType](./setcredentialsmethodtype/) | Bağlantıyı (veya yeniden bağlanmayı) kurarken kullanılacak kimlik doğrulama yöntemini belirtir. |
| [GetBackgroundRefresh](./getbackgroundrefresh/) | Bağlantının arka planda (eşzamansız) yenilenip yenilenemeyeceğini gösterir. Bağlantının tercih edilen kullanım şekli arka planda eşzamansız yenileme ise doğru; ön planda eşzamanlı yenileme ise yanlış. |
| [SetBackgroundRefresh](./setbackgroundrefresh/) | Bağlantının arka planda (eşzamansız) yenilenip yenilenemeyeceğini gösterir. Bağlantının tercih edilen kullanım şekli arka planda eşzamansız yenileme ise doğru; ön planda eşzamanlı yenileme ise yanlış. |
| [GetParameters](./getparameters/) | ODBC veya web sorgusu için ConnectionParameterCollection'ı alır. |
| [GetConnectionFile](./getconnectionfile/) | Bağlantı dosyasını alır. |
