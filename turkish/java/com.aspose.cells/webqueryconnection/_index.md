---
title: "WebQueryConnection"
second_title: "Aspose.Cells for Java API Referansı"
description: "Web sorgu kaynağı için özellikleri belirtir."
type: docs
url: /tr/java/com.aspose.cells/webqueryconnection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ExternalConnection](../../com.aspose.cells/externalconnection)
```
public class WebQueryConnection extends ExternalConnection
```

Bir web sorgu kaynağı için özellikleri belirtir. Bir web sorgusu, HTML tablolarından veri alır ve ayrıca parametreleri ve parametre öğelerini dahil ederek HTML oluşturulurken web sunucusu tarafından işlenecek HTTP \"Get\" parametrelerini de sağlayabilir.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackgroundRefresh()](#getBackgroundRefresh--) | Bağlantının arka planda (asenkron olarak) yenilenip yenilenemeyeceğini gösterir. |
| [getClass()](#getClass--) |  |
| [getClassType()](#getClassType--) | Bu [ExternalConnection](../../com.aspose.cells/externalconnection) nesnesinin türünü alır. |
| [getCommand()](#getCommand--) | Veri sağlayıcı API'sine iletilecek, dış kaynağa etkileşimde bulunarak veri almak için kullanılan veritabanı komutunu içeren dize |
| [getCommandType()](#getCommandType--) | OLE DB komut türünü belirtir. 1. |
| [getConnectionDescription()](#getConnectionDescription--) | Bu bağlantı için kullanıcı açıklamasını belirtir |
| [getConnectionFile()](#getConnectionFile--) | Bağlantı dosyasını alır. |
| [getConnectionId()](#getConnectionId--) | Bu bağlantının benzersiz tanımlayıcısını belirtir. |
| [getConnectionString()](#getConnectionString--) | Bağlantı bilgi dizesi, bir OLE DB veya ODBC veri kaynağıyla iletişim kurmak için kullanılır. |
| [getCredentials()](#getCredentials--) | Bağlantı kurulurken (veya yeniden kurulurken) kullanılacak kimlik doğrulama yöntemini belirtir. |
| [getCredentialsMethodType()](#getCredentialsMethodType--) | Bağlantı kurulurken (veya yeniden kurulurken) kullanılacak kimlik doğrulama yöntemini belirtir. |
| [getEditPage()](#getEditPage--) | Web sorgu verilerini gösteren kullanıcıya yönelik web sayfasının URL'si. |
| [getEditWebPage()](#getEditWebPage--) | Web sorgu verilerini gösteren kullanıcıya yönelik web sayfasının URL'si. |
| [getHtmlFormat()](#getHtmlFormat--) | Web sorgu verileri çalışma sayfasına getirildiğinde HTML kaynağından gelen biçimlendirme nasıl ele alınır. |
| [getId()](#getId--) | Bağlantının kimliğini alır. |
| [getKeepAlive()](#getKeepAlive--) | Elektronik tablo uygulamasının bağlantıyı açık tutmak için çaba göstermesi gerektiğinde doğru. |
| [getName()](#getName--) | Bağlantının adını belirtir. |
| [getOdcFile()](#getOdcFile--) | Bu bağlantının oluşturulduğu dış bağlantı dosyasının tam yolunu belirtir. |
| [getOnlyUseConnectionFile()](#getOnlyUseConnectionFile--) | Bağlantı yenilendiğinde elektronik tablo uygulamasının, odcFile özniteliğiyle belirtilen dış bağlantı dosyasındaki bağlantı bilgilerini her zaman ve yalnızca kullanıp kullanmayacağını gösterir. |
| [getParameters()](#getParameters--) | Bir ODBC veya web sorgusu için [ConnectionParameterCollection](../../com.aspose.cells/connectionparametercollection) alır. |
| [getPost()](#getPost--) | Web sorgusundan veri döndürmek için veri girişi yapılan web sunucusuna post yöntemiyle kullanılan dizeyi alır veya ayarlar. |
| [getPowerQueryFormula()](#getPowerQueryFormula--) | Power Query formülünün tanımını alır. |
| [getReconnectionMethod()](#getReconnectionMethod--) | Bir bağlantı başarısız olduğunda elektronik tablo uygulamasının ne yapması gerektiğini belirtir. |
| [getReconnectionMethodType()](#getReconnectionMethodType--) | Bir bağlantı başarısız olduğunda elektronik tablo uygulamasının ne yapması gerektiğini belirtir. |
| [getRefreshInternal()](#getRefreshInternal--) | Bağlantının otomatik yenilemeleri arasındaki dakika sayısını belirtir. |
| [getRefreshOnLoad()](#getRefreshOnLoad--) | Dosya açıldığında bu bağlantının yenilenmesi gerekiyorsa doğru; aksi takdirde yanlış. |
| [getSSOId()](#getSSOId--) | Ara bir spreadsheetML sunucusu ile dış veri kaynağı arasında kimlik doğrulama için kullanılan Tek Oturum Açma (SSO) tanımlayıcısı. |
| [getSaveData()](#getSaveData--) | Bağlantı üzerinden alınan dış verinin bir tabloyu doldurmak için çalışma kitabıyla birlikte kaydedilmesi gerekiyorsa doğru; aksi takdirde yanlış. |
| [getSavePassword()](#getSavePassword--) | Parolanın bağlantı dizesinin bir parçası olarak kaydedilmesi gerekiyorsa doğru; aksi takdirde Yanlış. |
| [getSecondCommand()](#getSecondCommand--) | PivotTable sunucu tabanlı sayfa alanları kullanıldığında kalıcı olan ikinci komut metni dizesini belirtir. |
| [getSourceFile()](#getSourceFile--) | Harici veri kaynağı dosya tabanlı olduğunda kullanılır. |
| [getSourceType()](#getSourceType--) | Harici bağlantı DataSource türünü alır. |
| [getType()](#getType--) | Harici bağlantı DataSource türünü alır. |
| [getUrl()](#getUrl--) | Harici verileri yenilemek için kullanılacak URL. |
| [hashCode()](#hashCode--) |  |
| [isConsecutive()](#isConsecutive--) | Ardışık ayırıcıların tek bir ayırıcı olarak ele alınıp alınmayacağını gösteren işaret. |
| [isDeleted()](#isDeleted--) | İlgili çalışma kitabı bağlantısının silinip silinmediğini gösterir. |
| [isHtmlTables()](#isHtmlTables--) | Web sorgularının yalnızca HTML tablolarında çalışıp çalışmayacağını gösteren işaret. |
| [isNew()](#isNew--) | Bağlantı ilk kez yenilenmemişse doğru; aksi takdirde yanlış. |
| [isParsePre()](#isParsePre--) | Web sayfasındaki HTML PRE etiketleri içinde bulunan verilerin, sayfa bir sorgu tablosuna içe aktarıldığında sütunlara ayrılıp ayrılmayacağını gösteren işaret. |
| [isSameSettings()](#isSameSettings--) | PRE bloğu içindeki tüm tabloların, ilk satırın aynı genişlik ayarlarıyla ayrılıp ayrılmayacağını gösteren işaret. |
| [isTextDates()](#isTextDates--) | Tarihlerin, çalışma sayfasındaki hücrelere tarih olarak değil metin olarak içe aktarılıp aktarılmayacağını gösteren işaret. |
| [isXl2000()](#isXl2000--) | Bu bayrak, daha eski mevcut elektronik tablo dosyalarıyla geriye dönük uyumluluk sağlamak için bulunur ve bu web sorgusu Microsoft Excel 2000 veya daha yeni bir elektronik tablo uygulamasında yenilendiğinde true olarak ayarlanır. |
| [isXl97()](#isXl97--) | Bu bayrak, daha eski mevcut elektronik tablo dosyalarıyla geriye dönük uyumluluk sağlamak için bulunur ve bu web sorgusu Microsoft Excel 97'de oluşturulduğunda true olarak ayarlanır. |
| [isXml()](#isXml--) | Web sorgusu kaynağı XML ise true, aksi takdirde false. |
| [isXmlSourceData()](#isXmlSourceData--) | HTML tablosu yerine XML kaynak verisinin içe aktarılması gerektiğini gösteren bayrak. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackgroundRefresh(boolean value)](#setBackgroundRefresh-boolean-) | Bağlantının arka planda (asenkron olarak) yenilenip yenilenemeyeceğini gösterir. |
| [setCommand(String value)](#setCommand-java.lang.String-) | Veri sağlayıcı API'sine iletilecek, dış kaynağa etkileşimde bulunarak veri almak için kullanılan veritabanı komutunu içeren dize |
| [setCommandType(int value)](#setCommandType-int-) | OLE DB komut türünü belirtir. 1. |
| [setConnectionDescription(String value)](#setConnectionDescription-java.lang.String-) | Bu bağlantı için kullanıcı açıklamasını belirtir |
| [setConnectionString(String value)](#setConnectionString-java.lang.String-) | Bağlantı bilgi dizesi, bir OLE DB veya ODBC veri kaynağıyla iletişim kurmak için kullanılır. |
| [setConsecutive(boolean value)](#setConsecutive-boolean-) | Ardışık ayırıcıların tek bir ayırıcı olarak ele alınıp alınmayacağını gösteren işaret. |
| [setCredentials(int value)](#setCredentials-int-) | Bağlantı kurulurken (veya yeniden kurulurken) kullanılacak kimlik doğrulama yöntemini belirtir. |
| [setCredentialsMethodType(int value)](#setCredentialsMethodType-int-) | Bağlantı kurulurken (veya yeniden kurulurken) kullanılacak kimlik doğrulama yöntemini belirtir. |
| [setDeleted(boolean value)](#setDeleted-boolean-) | İlgili çalışma kitabı bağlantısının silinip silinmediğini gösterir. |
| [setEditPage(String value)](#setEditPage-java.lang.String-) | Web sorgu verilerini gösteren kullanıcıya yönelik web sayfasının URL'si. |
| [setEditWebPage(String value)](#setEditWebPage-java.lang.String-) | Web sorgu verilerini gösteren kullanıcıya yönelik web sayfasının URL'si. |
| [setHtmlFormat(int value)](#setHtmlFormat-int-) | Web sorgu verileri çalışma sayfasına getirildiğinde HTML kaynağından gelen biçimlendirme nasıl ele alınır. |
| [setHtmlTables(boolean value)](#setHtmlTables-boolean-) | Web sorgularının yalnızca HTML tablolarında çalışıp çalışmayacağını gösteren işaret. |
| [setKeepAlive(boolean value)](#setKeepAlive-boolean-) | Elektronik tablo uygulamasının bağlantıyı açık tutmak için çaba göstermesi gerektiğinde doğru. |
| [setName(String value)](#setName-java.lang.String-) | Bağlantının adını belirtir. |
| [setNew(boolean value)](#setNew-boolean-) | Bağlantı ilk kez yenilenmemişse doğru; aksi takdirde yanlış. |
| [setOdcFile(String value)](#setOdcFile-java.lang.String-) | Bu bağlantının oluşturulduğu dış bağlantı dosyasının tam yolunu belirtir. |
| [setOnlyUseConnectionFile(boolean value)](#setOnlyUseConnectionFile-boolean-) | Bağlantı yenilendiğinde elektronik tablo uygulamasının, odcFile özniteliğiyle belirtilen dış bağlantı dosyasındaki bağlantı bilgilerini her zaman ve yalnızca kullanıp kullanmayacağını gösterir. |
| [setParsePre(boolean value)](#setParsePre-boolean-) | Web sayfasındaki HTML PRE etiketleri içinde bulunan verilerin, sayfa bir sorgu tablosuna içe aktarıldığında sütunlara ayrılıp ayrılmayacağını gösteren işaret. |
| [setPost(String value)](#setPost-java.lang.String-) | Web sorgusundan veri döndürmek için veri girişi yapılan web sunucusuna post yöntemiyle kullanılan dizeyi alır veya ayarlar. |
| [setReconnectionMethod(int value)](#setReconnectionMethod-int-) | Bir bağlantı başarısız olduğunda elektronik tablo uygulamasının ne yapması gerektiğini belirtir. |
| [setReconnectionMethodType(int value)](#setReconnectionMethodType-int-) | Bir bağlantı başarısız olduğunda elektronik tablo uygulamasının ne yapması gerektiğini belirtir. |
| [setRefreshInternal(int value)](#setRefreshInternal-int-) | Bağlantının otomatik yenilemeleri arasındaki dakika sayısını belirtir. |
| [setRefreshOnLoad(boolean value)](#setRefreshOnLoad-boolean-) | Dosya açıldığında bu bağlantının yenilenmesi gerekiyorsa doğru; aksi takdirde yanlış. |
| [setSSOId(String value)](#setSSOId-java.lang.String-) | Ara bir spreadsheetML sunucusu ile dış veri kaynağı arasında kimlik doğrulama için kullanılan Tek Oturum Açma (SSO) tanımlayıcısı. |
| [setSameSettings(boolean value)](#setSameSettings-boolean-) | PRE bloğu içindeki tüm tabloların, ilk satırın aynı genişlik ayarlarıyla ayrılıp ayrılmayacağını gösteren işaret. |
| [setSaveData(boolean value)](#setSaveData-boolean-) | Bağlantı üzerinden alınan dış verinin bir tabloyu doldurmak için çalışma kitabıyla birlikte kaydedilmesi gerekiyorsa doğru; aksi takdirde yanlış. |
| [setSavePassword(boolean value)](#setSavePassword-boolean-) | Parolanın bağlantı dizesinin bir parçası olarak kaydedilmesi gerekiyorsa doğru; aksi takdirde Yanlış. |
| [setSecondCommand(String value)](#setSecondCommand-java.lang.String-) | PivotTable sunucu tabanlı sayfa alanları kullanıldığında kalıcı olan ikinci komut metni dizesini belirtir. |
| [setSourceFile(String value)](#setSourceFile-java.lang.String-) | Harici veri kaynağı dosya tabanlı olduğunda kullanılır. |
| [setSourceType(int value)](#setSourceType-int-) | Harici bağlantı DataSource türünü ayarlar. |
| [setTextDates(boolean value)](#setTextDates-boolean-) | Tarihlerin, çalışma sayfasındaki hücrelere tarih olarak değil metin olarak içe aktarılıp aktarılmayacağını gösteren işaret. |
| [setType(int value)](#setType-int-) | Harici bağlantı DataSource türünü ayarlar. |
| [setUrl(String value)](#setUrl-java.lang.String-) | Harici verileri yenilemek için kullanılacak URL. |
| [setXl2000(boolean value)](#setXl2000-boolean-) | Bu bayrak, daha eski mevcut elektronik tablo dosyalarıyla geriye dönük uyumluluk sağlamak için bulunur ve bu web sorgusu Microsoft Excel 2000 veya daha yeni bir elektronik tablo uygulamasında yenilendiğinde true olarak ayarlanır. |
| [setXl97(boolean value)](#setXl97-boolean-) | Bu bayrak, daha eski mevcut elektronik tablo dosyalarıyla geriye dönük uyumluluk sağlamak için bulunur ve bu web sorgusu Microsoft Excel 97'de oluşturulduğunda true olarak ayarlanır. |
| [setXml(boolean value)](#setXml-boolean-) | Web sorgusu kaynağı XML ise true, aksi takdirde false. |
| [setXmlSourceData(boolean value)](#setXmlSourceData-boolean-) | HTML tablosu yerine XML kaynak verisinin içe aktarılması gerektiğini gösteren bayrak. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getBackgroundRefresh() {#getBackgroundRefresh--}
```
public boolean getBackgroundRefresh()
```


Bağlantının arka planda (asenkron olarak) yenilenip yenilenemeyeceğini gösterir. Bağlantının tercih edilen kullanım şekli arka planda asenkron yenileme ise true; ön planda senkron yenileme ise false.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getClassType() {#getClassType--}
```
public int getClassType()
```


Bu [ExternalConnection](../../com.aspose.cells/externalconnection) nesnesinin türünü alır.

Bakınız [ExternalConnectionClassType](../../com.aspose.cells/externalconnectionclasstype).

**Returns:**
int
### getCommand() {#getCommand--}
```
public String getCommand()
```


Veri sağlayıcı API'sine iletilecek, dış kaynağa etkileşimde bulunarak veri almak için kullanılan veritabanı komutunu içeren dize

**Returns:**
java.lang.String
### getCommandType() {#getCommandType--}
```
public int getCommandType()
```


OLE DB komut türünü belirtir. 1. Sorgu bir küp adı belirtir 2. Sorgu bir SQL ifadesi belirtir 3. Sorgu bir tablo adı belirtir 4. Sorgu varsayılan bilgilerin verildiğini belirtir ve yorumlama sağlayıcıya bırakılır. 5. Sorgu web tabanlı Liste Veri Sağlayıcısına yöneliktir.

Bakınız [OLEDBCommandType](../../com.aspose.cells/oledbcommandtype).

**Returns:**
int
### getConnectionDescription() {#getConnectionDescription--}
```
public String getConnectionDescription()
```


Bu bağlantı için kullanıcı açıklamasını belirtir

**Returns:**
java.lang.String
### getConnectionFile() {#getConnectionFile--}
```
public String getConnectionFile()
```


Bağlantı dosyasını alır.

**Returns:**
java.lang.String
### getConnectionId() {#getConnectionId--}
```
public int getConnectionId()
```


Bu bağlantının benzersiz tanımlayıcısını belirtir.

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırılmıştır. Bunun yerine lütfen ExternalConnection.Id özelliğini kullanın. Bu özellik Ekim 2024'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
int
### getConnectionString() {#getConnectionString--}
```
public String getConnectionString()
```


Bağlantı bilgi dizesi, bir OLE DB veya ODBC veri kaynağıyla iletişim kurmak için kullanılır.

**Returns:**
java.lang.String
### getCredentials() {#getCredentials--}
```
public int getCredentials()
```


Bağlantı kurulurken (veya yeniden kurulurken) kullanılacak kimlik doğrulama yöntemini belirtir.

Bakınız [CredentialsMethodType](../../com.aspose.cells/credentialsmethodtype).

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırılmıştır. Bunun yerine lütfen ExternalConnection.CredentialsMethodType özelliğini kullanın. Bu özellik Ekim 2017'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
int
### getCredentialsMethodType() {#getCredentialsMethodType--}
```
public int getCredentialsMethodType()
```


Bağlantı kurulurken (veya yeniden kurulurken) kullanılacak kimlik doğrulama yöntemini belirtir.

Bakınız [CredentialsMethodType](../../com.aspose.cells/credentialsmethodtype).

**Returns:**
int
### getEditPage() {#getEditPage--}
```
public String getEditPage()
```


Web sorgusu verilerini gösteren kullanıcıya yönelik web sayfasının URL'si. sourceData=\"true\" ve url bir XML dosyasına yönlendirildiğinde bu URL saklanır. Böylece kullanıcıya yönelik sayfa UI'da gösterilebilir ve XML verisi arka planda alınabilir.

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırılmıştır. Bunun yerine lütfen WebQueryConnection.EditWebPage özelliğini kullanın. Bu özellik Ekim 2017'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
java.lang.String
### getEditWebPage() {#getEditWebPage--}
```
public String getEditWebPage()
```


Web sorgusu verilerini gösteren kullanıcıya yönelik web sayfasının URL'si. sourceData=\"true\" ve url bir XML dosyasına yönlendirildiğinde bu URL saklanır. Böylece kullanıcıya yönelik sayfa UI'da gösterilebilir ve XML verisi arka planda alınabilir.

**Returns:**
java.lang.String
### getHtmlFormat() {#getHtmlFormat--}
```
public int getHtmlFormat()
```


Web sorgusu verileri çalışma sayfasına getirildiğinde HTML kaynağından gelen biçimlendirme nasıl ele alınır. sourceData true olduğunda geçerlidir.

Bakınız [HtmlFormatHandlingType](../../com.aspose.cells/htmlformathandlingtype).

**Returns:**
int
### getId() {#getId--}
```
public int getId()
```


Bağlantının kimliğini alır.

**Returns:**
int
### getKeepAlive() {#getKeepAlive--}
```
public boolean getKeepAlive()
```


Bağlantının açık tutulması için elektronik tablo uygulamasının çaba göstermesi gerektiğinde true. False olduğunda, uygulama bilgiyi aldıktan sonra bağlantıyı kapatmalıdır.

**Returns:**
boolean
### getName() {#getName--}
```
public String getName()
```


Bağlantının adını belirtir. Her bağlantının benzersiz bir adı olmalıdır.

**Returns:**
java.lang.String
### getOdcFile() {#getOdcFile--}
```
public String getOdcFile()
```


Bu bağlantının oluşturulduğu harici bağlantı dosyasının tam yolunu belirtir. Veri yenileme girişimi sırasında bir bağlantı başarısız olursa ve reconnectionMethod=1 ise, elektronik tablo uygulaması çalışma kitabına gömülü bağlantı nesnesi yerine harici bağlantı dosyasındaki bilgileri kullanarak tekrar deneyecektir.

**Returns:**
java.lang.String
### getOnlyUseConnectionFile() {#getOnlyUseConnectionFile--}
```
public boolean getOnlyUseConnectionFile()
```


Bağlantı yenilendiğinde elektronik tablo uygulamasının her zaman ve yalnızca odcFile özniteliğiyle belirtilen harici bağlantı dosyasındaki bağlantı bilgilerini kullanıp kullanmayacağını gösterir. False ise, uygulama reconnectionMethod özniteliğiyle belirtilen prosedürü izlemelidir.

**Returns:**
boolean
### getParameters() {#getParameters--}
```
public ConnectionParameterCollection getParameters()
```


Bir ODBC veya web sorgusu için [ConnectionParameterCollection](../../com.aspose.cells/connectionparametercollection) alır.

**Returns:**
[ConnectionParameterCollection](../../com.aspose.cells/connectionparametercollection)
### getPost() {#getPost--}
```
public String getPost()
```


Web sorgusundan veri döndürmek için veri girişi yapılan web sunucusuna post yöntemiyle kullanılan dizeyi alır veya ayarlar.

**Returns:**
java.lang.String
### getPowerQueryFormula() {#getPowerQueryFormula--}
```
public PowerQueryFormula getPowerQueryFormula()
```


Power Query formülünün tanımını alır.

**Returns:**
[PowerQueryFormula](../../com.aspose.cells/powerqueryformula)
### getReconnectionMethod() {#getReconnectionMethod--}
```
public int getReconnectionMethod()
```


Bir bağlantı başarısız olduğunda elektronik tablo uygulamasının ne yapması gerektiğini belirtir. Varsayılan değer ReConnectionMethodType.Required'tir.

Bakınız [ReConnectionMethodType](../../com.aspose.cells/reconnectionmethodtype).

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırılmıştır. Bunun yerine lütfen ExternalConnection.ReconnectionMethodType özelliğini kullanın. Bu özellik Ekim 2017'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
int
### getReconnectionMethodType() {#getReconnectionMethodType--}
```
public int getReconnectionMethodType()
```


Bir bağlantı başarısız olduğunda elektronik tablo uygulamasının ne yapması gerektiğini belirtir. Varsayılan değer ReConnectionMethodType.Required'tir.

Bakınız [ReConnectionMethodType](../../com.aspose.cells/reconnectionmethodtype).

**Returns:**
int
### getRefreshInternal() {#getRefreshInternal--}
```
public int getRefreshInternal()
```


Bağlantının otomatik yenilemeleri arasındaki dakika sayısını belirtir.

**Returns:**
int
### getRefreshOnLoad() {#getRefreshOnLoad--}
```
public boolean getRefreshOnLoad()
```


Dosya açıldığında bu bağlantının yenilenmesi gerekiyorsa doğru; aksi takdirde yanlış.

**Returns:**
boolean
### getSSOId() {#getSSOId--}
```
public String getSSOId()
```


Ara bir spreadsheetML sunucusu ile dış veri kaynağı arasında kimlik doğrulama için kullanılan Tek Oturum Açma (SSO) tanımlayıcısı.

**Returns:**
java.lang.String
### getSaveData() {#getSaveData--}
```
public boolean getSaveData()
```


Bağlantı üzerinden alınan dış verinin bir tabloyu doldurmak için çalışma kitabıyla birlikte kaydedilmesi gerekiyorsa doğru; aksi takdirde yanlış.

**Returns:**
boolean
### getSavePassword() {#getSavePassword--}
```
public boolean getSavePassword()
```


Parolanın bağlantı dizesinin bir parçası olarak kaydedilmesi gerekiyorsa doğru; aksi takdirde Yanlış.

**Returns:**
boolean
### getSecondCommand() {#getSecondCommand--}
```
public String getSecondCommand()
```


PivotTable sunucu tabanlı sayfa alanları kullanıldığında kalıcı olan ikinci komut metni dizesini belirtir. ODBC bağlantıları için serverCommand genellikle command'tan daha geniş bir sorgudur (ilki WHERE koşulu içermez). Bu iki komuta (Command ve ServerCommand) dayanarak parametre UI'si doldurulabilir ve parametreli sorgular oluşturulabilir.

**Returns:**
java.lang.String
### getSourceFile() {#getSourceFile--}
```
public String getSourceFile()
```


Harici veri kaynağı dosya tabanlı olduğunda kullanılır. Böyle bir veri kaynağına bağlantı başarısız olduğunda, elektronik tablo uygulaması bu dosyaya doğrudan bağlanmayı dener. URI veya sistem‑özel dosya yolu gösterimiyle ifade edilebilir.

**Returns:**
java.lang.String
### getSourceType() {#getSourceType--}
```
public int getSourceType()
```


Harici bağlantı DataSource türünü alır.

Bakın [ConnectionDataSourceType](../../com.aspose.cells/connectiondatasourcetype).

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Harici bağlantı DataSource türünü alır.

Bakın [ConnectionDataSourceType](../../com.aspose.cells/connectiondatasourcetype).

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırıldı. Bunun yerine lütfen ExternalConnection.SourceType özelliğini kullanın. Bu özellik Ekim 2024'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
int
### getUrl() {#getUrl--}
```
public String getUrl()
```


Harici verileri yenilemek için kullanılacak URL.

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isConsecutive() {#isConsecutive--}
```
public boolean isConsecutive()
```


Ardışık ayırıcıların tek bir ayırıcı olarak ele alınıp alınmayacağını gösteren işaret.

**Returns:**
boolean
### isDeleted() {#isDeleted--}
```
public boolean isDeleted()
```


İlgili çalışma kitabı bağlantısının silinip silinmediğini gösterir. Bağlantı silinmişse true; aksi takdirde false.

**Returns:**
boolean
### isHtmlTables() {#isHtmlTables--}
```
public boolean isHtmlTables()
```


Web sorgularının yalnızca HTML tablolarında çalışıp çalışmayacağını gösteren işaret.

**Returns:**
boolean
### isNew() {#isNew--}
```
public boolean isNew()
```


Bağlantı ilk kez yenilenmemişse true; aksi takdirde false. Bu durum, kullanıcının sorgu tamamlanmadan dosyayı kaydetmesi durumunda ortaya çıkabilir.

**Returns:**
boolean
### isParsePre() {#isParsePre--}
```
public boolean isParsePre()
```


Web sayfasındaki HTML PRE etiketleri içinde bulunan verilerin, sayfa bir sorgu tablosuna içe aktarıldığında sütunlara ayrılıp ayrılmayacağını gösteren işaret.

**Returns:**
boolean
### isSameSettings() {#isSameSettings--}
```
public boolean isSameSettings()
```


PRE bloğu içindeki tüm tabloların, ilk satırın aynı genişlik ayarlarıyla ayrılıp ayrılmayacağını gösteren işaret.

**Returns:**
boolean
### isTextDates() {#isTextDates--}
```
public boolean isTextDates()
```


Tarihlerin, çalışma sayfasındaki hücrelere tarih olarak değil metin olarak içe aktarılıp aktarılmayacağını gösteren işaret.

**Returns:**
boolean
### isXl2000() {#isXl2000--}
```
public boolean isXl2000()
```


Bu bayrak, daha eski mevcut elektronik tablo dosyalarıyla geriye dönük uyumluluk sağlamak için bulunur ve bu web sorgusu Microsoft Excel 2000 veya daha yeni bir elektronik tablo uygulamasında yenilendiğinde true olarak ayarlanır. Bu, göz ardı edilebilecek isteğe bağlı bir özelliktir.

**Returns:**
boolean
### isXl97() {#isXl97--}
```
public boolean isXl97()
```


Bu bayrak, daha eski mevcut elektronik tablo dosyalarıyla geriye dönük uyumluluk sağlamak için bulunur ve bu web sorgusu Microsoft Excel 97'de oluşturulduğunda true olarak ayarlanır. Bu, göz ardı edilebilecek isteğe bağlı bir özelliktir.

**Returns:**
boolean
### isXml() {#isXml--}
```
public boolean isXml()
```


Web sorgusu kaynağı XML ise true, aksi takdirde false.

**Returns:**
boolean
### isXmlSourceData() {#isXmlSourceData--}
```
public boolean isXmlSourceData()
```


HTML tablosu yerine XML kaynak verisinin içe aktarılması gerektiğini gösteren bayrak.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setBackgroundRefresh(boolean value) {#setBackgroundRefresh-boolean-}
```
public void setBackgroundRefresh(boolean value)
```


Bağlantının arka planda (asenkron olarak) yenilenip yenilenemeyeceğini gösterir. Bağlantının tercih edilen kullanım şekli arka planda asenkron yenileme ise true; ön planda senkron yenileme ise false.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setCommand(String value) {#setCommand-java.lang.String-}
```
public void setCommand(String value)
```


Veri sağlayıcı API'sine iletilecek, dış kaynağa etkileşimde bulunarak veri almak için kullanılan veritabanı komutunu içeren dize

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setCommandType(int value) {#setCommandType-int-}
```
public void setCommandType(int value)
```


OLE DB komut türünü belirtir. 1. Sorgu bir küp adı belirtir 2. Sorgu bir SQL ifadesi belirtir 3. Sorgu bir tablo adı belirtir 4. Sorgu varsayılan bilgilerin verildiğini belirtir ve yorumlama sağlayıcıya bırakılır. 5. Sorgu web tabanlı Liste Veri Sağlayıcısına yöneliktir.

Bakınız [OLEDBCommandType](../../com.aspose.cells/oledbcommandtype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setConnectionDescription(String value) {#setConnectionDescription-java.lang.String-}
```
public void setConnectionDescription(String value)
```


Bu bağlantı için kullanıcı açıklamasını belirtir

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setConnectionString(String value) {#setConnectionString-java.lang.String-}
```
public void setConnectionString(String value)
```


Bağlantı bilgi dizesi, bir OLE DB veya ODBC veri kaynağıyla iletişim kurmak için kullanılır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setConsecutive(boolean value) {#setConsecutive-boolean-}
```
public void setConsecutive(boolean value)
```


Ardışık ayırıcıların tek bir ayırıcı olarak ele alınıp alınmayacağını gösteren işaret.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setCredentials(int value) {#setCredentials-int-}
```
public void setCredentials(int value)
```


Bağlantı kurulurken (veya yeniden kurulurken) kullanılacak kimlik doğrulama yöntemini belirtir.

Bakınız [CredentialsMethodType](../../com.aspose.cells/credentialsmethodtype).

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırılmıştır. Bunun yerine lütfen ExternalConnection.CredentialsMethodType özelliğini kullanın. Bu özellik Ekim 2017'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setCredentialsMethodType(int value) {#setCredentialsMethodType-int-}
```
public void setCredentialsMethodType(int value)
```


Bağlantı kurulurken (veya yeniden kurulurken) kullanılacak kimlik doğrulama yöntemini belirtir.

Bakınız [CredentialsMethodType](../../com.aspose.cells/credentialsmethodtype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setDeleted(boolean value) {#setDeleted-boolean-}
```
public void setDeleted(boolean value)
```


İlgili çalışma kitabı bağlantısının silinip silinmediğini gösterir. Bağlantı silinmişse true; aksi takdirde false.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setEditPage(String value) {#setEditPage-java.lang.String-}
```
public void setEditPage(String value)
```


Web sorgusu verilerini gösteren kullanıcıya yönelik web sayfasının URL'si. sourceData=\"true\" ve url bir XML dosyasına yönlendirildiğinde bu URL saklanır. Böylece kullanıcıya yönelik sayfa UI'da gösterilebilir ve XML verisi arka planda alınabilir.

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırılmıştır. Bunun yerine lütfen WebQueryConnection.EditWebPage özelliğini kullanın. Bu özellik Ekim 2017'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setEditWebPage(String value) {#setEditWebPage-java.lang.String-}
```
public void setEditWebPage(String value)
```


Web sorgusu verilerini gösteren kullanıcıya yönelik web sayfasının URL'si. sourceData=\"true\" ve url bir XML dosyasına yönlendirildiğinde bu URL saklanır. Böylece kullanıcıya yönelik sayfa UI'da gösterilebilir ve XML verisi arka planda alınabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setHtmlFormat(int value) {#setHtmlFormat-int-}
```
public void setHtmlFormat(int value)
```


Web sorgusu verileri çalışma sayfasına getirildiğinde HTML kaynağından gelen biçimlendirme nasıl ele alınır. sourceData true olduğunda geçerlidir.

Bakınız [HtmlFormatHandlingType](../../com.aspose.cells/htmlformathandlingtype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setHtmlTables(boolean value) {#setHtmlTables-boolean-}
```
public void setHtmlTables(boolean value)
```


Web sorgularının yalnızca HTML tablolarında çalışıp çalışmayacağını gösteren işaret.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setKeepAlive(boolean value) {#setKeepAlive-boolean-}
```
public void setKeepAlive(boolean value)
```


Bağlantının açık tutulması için elektronik tablo uygulamasının çaba göstermesi gerektiğinde true. False olduğunda, uygulama bilgiyi aldıktan sonra bağlantıyı kapatmalıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Bağlantının adını belirtir. Her bağlantının benzersiz bir adı olmalıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setNew(boolean value) {#setNew-boolean-}
```
public void setNew(boolean value)
```


Bağlantı ilk kez yenilenmemişse true; aksi takdirde false. Bu durum, kullanıcının sorgu tamamlanmadan dosyayı kaydetmesi durumunda ortaya çıkabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setOdcFile(String value) {#setOdcFile-java.lang.String-}
```
public void setOdcFile(String value)
```


Bu bağlantının oluşturulduğu harici bağlantı dosyasının tam yolunu belirtir. Veri yenileme girişimi sırasında bir bağlantı başarısız olursa ve reconnectionMethod=1 ise, elektronik tablo uygulaması çalışma kitabına gömülü bağlantı nesnesi yerine harici bağlantı dosyasındaki bilgileri kullanarak tekrar deneyecektir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setOnlyUseConnectionFile(boolean value) {#setOnlyUseConnectionFile-boolean-}
```
public void setOnlyUseConnectionFile(boolean value)
```


Bağlantı yenilendiğinde elektronik tablo uygulamasının her zaman ve yalnızca odcFile özniteliğiyle belirtilen harici bağlantı dosyasındaki bağlantı bilgilerini kullanıp kullanmayacağını gösterir. False ise, uygulama reconnectionMethod özniteliğiyle belirtilen prosedürü izlemelidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setParsePre(boolean value) {#setParsePre-boolean-}
```
public void setParsePre(boolean value)
```


Web sayfasındaki HTML PRE etiketleri içinde bulunan verilerin, sayfa bir sorgu tablosuna içe aktarıldığında sütunlara ayrılıp ayrılmayacağını gösteren işaret.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setPost(String value) {#setPost-java.lang.String-}
```
public void setPost(String value)
```


Web sorgusundan veri döndürmek için veri girişi yapılan web sunucusuna post yöntemiyle kullanılan dizeyi alır veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setReconnectionMethod(int value) {#setReconnectionMethod-int-}
```
public void setReconnectionMethod(int value)
```


Bir bağlantı başarısız olduğunda elektronik tablo uygulamasının ne yapması gerektiğini belirtir. Varsayılan değer ReConnectionMethodType.Required'tir.

Bakınız [ReConnectionMethodType](../../com.aspose.cells/reconnectionmethodtype).

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırılmıştır. Bunun yerine lütfen ExternalConnection.ReconnectionMethodType özelliğini kullanın. Bu özellik Ekim 2017'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setReconnectionMethodType(int value) {#setReconnectionMethodType-int-}
```
public void setReconnectionMethodType(int value)
```


Bir bağlantı başarısız olduğunda elektronik tablo uygulamasının ne yapması gerektiğini belirtir. Varsayılan değer ReConnectionMethodType.Required'tir.

Bakınız [ReConnectionMethodType](../../com.aspose.cells/reconnectionmethodtype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setRefreshInternal(int value) {#setRefreshInternal-int-}
```
public void setRefreshInternal(int value)
```


Bağlantının otomatik yenilemeleri arasındaki dakika sayısını belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setRefreshOnLoad(boolean value) {#setRefreshOnLoad-boolean-}
```
public void setRefreshOnLoad(boolean value)
```


Dosya açıldığında bu bağlantının yenilenmesi gerekiyorsa doğru; aksi takdirde yanlış.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setSSOId(String value) {#setSSOId-java.lang.String-}
```
public void setSSOId(String value)
```


Ara bir spreadsheetML sunucusu ile dış veri kaynağı arasında kimlik doğrulama için kullanılan Tek Oturum Açma (SSO) tanımlayıcısı.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setSameSettings(boolean value) {#setSameSettings-boolean-}
```
public void setSameSettings(boolean value)
```


PRE bloğu içindeki tüm tabloların, ilk satırın aynı genişlik ayarlarıyla ayrılıp ayrılmayacağını gösteren işaret.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setSaveData(boolean value) {#setSaveData-boolean-}
```
public void setSaveData(boolean value)
```


Bağlantı üzerinden alınan dış verinin bir tabloyu doldurmak için çalışma kitabıyla birlikte kaydedilmesi gerekiyorsa doğru; aksi takdirde yanlış.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setSavePassword(boolean value) {#setSavePassword-boolean-}
```
public void setSavePassword(boolean value)
```


Parolanın bağlantı dizesinin bir parçası olarak kaydedilmesi gerekiyorsa doğru; aksi takdirde Yanlış.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setSecondCommand(String value) {#setSecondCommand-java.lang.String-}
```
public void setSecondCommand(String value)
```


PivotTable sunucu tabanlı sayfa alanları kullanıldığında kalıcı olan ikinci komut metni dizesini belirtir. ODBC bağlantıları için serverCommand genellikle command'tan daha geniş bir sorgudur (ilki WHERE koşulu içermez). Bu iki komuta (Command ve ServerCommand) dayanarak parametre UI'si doldurulabilir ve parametreli sorgular oluşturulabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setSourceFile(String value) {#setSourceFile-java.lang.String-}
```
public void setSourceFile(String value)
```


Harici veri kaynağı dosya tabanlı olduğunda kullanılır. Böyle bir veri kaynağına bağlantı başarısız olduğunda, elektronik tablo uygulaması bu dosyaya doğrudan bağlanmayı dener. URI veya sistem‑özel dosya yolu gösterimiyle ifade edilebilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setSourceType(int value) {#setSourceType-int-}
```
public void setSourceType(int value)
```


Harici bağlantı DataSource türünü ayarlar.

Bakın [ConnectionDataSourceType](../../com.aspose.cells/connectiondatasourcetype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setTextDates(boolean value) {#setTextDates-boolean-}
```
public void setTextDates(boolean value)
```


Tarihlerin, çalışma sayfasındaki hücrelere tarih olarak değil metin olarak içe aktarılıp aktarılmayacağını gösteren işaret.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Harici bağlantı DataSource türünü ayarlar.

Bakın [ConnectionDataSourceType](../../com.aspose.cells/connectiondatasourcetype).

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırıldı. Bunun yerine lütfen ExternalConnection.SourceType özelliğini kullanın. Bu özellik Ekim 2024'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setUrl(String value) {#setUrl-java.lang.String-}
```
public void setUrl(String value)
```


Harici verileri yenilemek için kullanılacak URL.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setXl2000(boolean value) {#setXl2000-boolean-}
```
public void setXl2000(boolean value)
```


Bu bayrak, daha eski mevcut elektronik tablo dosyalarıyla geriye dönük uyumluluk sağlamak için bulunur ve bu web sorgusu Microsoft Excel 2000 veya daha yeni bir elektronik tablo uygulamasında yenilendiğinde true olarak ayarlanır. Bu, göz ardı edilebilecek isteğe bağlı bir özelliktir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setXl97(boolean value) {#setXl97-boolean-}
```
public void setXl97(boolean value)
```


Bu bayrak, daha eski mevcut elektronik tablo dosyalarıyla geriye dönük uyumluluk sağlamak için bulunur ve bu web sorgusu Microsoft Excel 97'de oluşturulduğunda true olarak ayarlanır. Bu, göz ardı edilebilecek isteğe bağlı bir özelliktir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setXml(boolean value) {#setXml-boolean-}
```
public void setXml(boolean value)
```


Web sorgusu kaynağı XML ise true, aksi takdirde false.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setXmlSourceData(boolean value) {#setXmlSourceData-boolean-}
```
public void setXmlSourceData(boolean value)
```


HTML tablosu yerine XML kaynak verisinin içe aktarılması gerektiğini gösteren bayrak.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

