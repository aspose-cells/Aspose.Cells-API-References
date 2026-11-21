---
title: "DataModelConnection"
second_title: "Aspose.Cells for Java API Referansı"
description: "Bir veri modeli bağlantısını belirtir"
type: docs
url: /tr/java/com.aspose.cells/datamodelconnection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ExternalConnection](../../com.aspose.cells/externalconnection)
```
public class DataModelConnection extends ExternalConnection
```

Bir veri modeli bağlantısını belirtir
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackgroundRefresh()](#getBackgroundRefresh--) | Bağlantının arka planda (asenkron olarak) yenilenip yenilenemeyeceğini gösterir. |
| [getClass()](#getClass--) |  |
| [getClassType()](#getClassType--) | Bu [ExternalConnection](../../com.aspose.cells/externalconnection) nesnesinin türünü alır. |
| [getCommand()](#getCommand--) | Veri sağlayıcı API'sine iletilecek, dış kaynağa etkileşimde bulunarak veri almak için kullanılan veritabanı komutunu içeren dize |
| [getCommandType()](#getCommandType--) | Döndürür [OLEDBCommandType](../../com.aspose.cells/oledbcommandtype) türü. |
| [getConnectionDescription()](#getConnectionDescription--) | Bu bağlantı için kullanıcı açıklamasını belirtir |
| [getConnectionFile()](#getConnectionFile--) | Bağlantı dosyasını alır. |
| [getConnectionId()](#getConnectionId--) | Bu bağlantının benzersiz tanımlayıcısını belirtir. |
| [getConnectionString()](#getConnectionString--) | Bağlantı bilgi dizesi, bir OLE DB veya ODBC veri kaynağıyla iletişim kurmak için kullanılır. |
| [getCredentials()](#getCredentials--) | Bağlantı kurulurken (veya yeniden kurulurken) kullanılacak kimlik doğrulama yöntemini belirtir. |
| [getCredentialsMethodType()](#getCredentialsMethodType--) | Bağlantı kurulurken (veya yeniden kurulurken) kullanılacak kimlik doğrulama yöntemini belirtir. |
| [getId()](#getId--) | Bağlantının kimliğini alır. |
| [getKeepAlive()](#getKeepAlive--) | Elektronik tablo uygulamasının bağlantıyı açık tutmak için çaba göstermesi gerektiğinde doğru. |
| [getName()](#getName--) | Bağlantının adını belirtir. |
| [getOdcFile()](#getOdcFile--) | Bu bağlantının oluşturulduğu dış bağlantı dosyasının tam yolunu belirtir. |
| [getOnlyUseConnectionFile()](#getOnlyUseConnectionFile--) | Bağlantı yenilendiğinde elektronik tablo uygulamasının, odcFile özniteliğiyle belirtilen dış bağlantı dosyasındaki bağlantı bilgilerini her zaman ve yalnızca kullanıp kullanmayacağını gösterir. |
| [getParameters()](#getParameters--) | Bir ODBC veya web sorgusu için [ConnectionParameterCollection](../../com.aspose.cells/connectionparametercollection) alır. |
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
| [hashCode()](#hashCode--) |  |
| [isDeleted()](#isDeleted--) | İlgili çalışma kitabı bağlantısının silinip silinmediğini gösterir. |
| [isNew()](#isNew--) | Bağlantı ilk kez yenilenmemişse doğru; aksi takdirde yanlış. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackgroundRefresh(boolean value)](#setBackgroundRefresh-boolean-) | Bağlantının arka planda (asenkron olarak) yenilenip yenilenemeyeceğini gösterir. |
| [setCommand(String value)](#setCommand-java.lang.String-) | Veri sağlayıcı API'sine iletilecek, dış kaynağa etkileşimde bulunarak veri almak için kullanılan veritabanı komutunu içeren dize |
| [setCommandType(int value)](#setCommandType-int-) | Döndürür [OLEDBCommandType](../../com.aspose.cells/oledbcommandtype) türü. |
| [setConnectionDescription(String value)](#setConnectionDescription-java.lang.String-) | Bu bağlantı için kullanıcı açıklamasını belirtir |
| [setConnectionString(String value)](#setConnectionString-java.lang.String-) | Bağlantı bilgi dizesi, bir OLE DB veya ODBC veri kaynağıyla iletişim kurmak için kullanılır. |
| [setCredentials(int value)](#setCredentials-int-) | Bağlantı kurulurken (veya yeniden kurulurken) kullanılacak kimlik doğrulama yöntemini belirtir. |
| [setCredentialsMethodType(int value)](#setCredentialsMethodType-int-) | Bağlantı kurulurken (veya yeniden kurulurken) kullanılacak kimlik doğrulama yöntemini belirtir. |
| [setDeleted(boolean value)](#setDeleted-boolean-) | İlgili çalışma kitabı bağlantısının silinip silinmediğini gösterir. |
| [setKeepAlive(boolean value)](#setKeepAlive-boolean-) | Elektronik tablo uygulamasının bağlantıyı açık tutmak için çaba göstermesi gerektiğinde doğru. |
| [setName(String value)](#setName-java.lang.String-) | Bağlantının adını belirtir. |
| [setNew(boolean value)](#setNew-boolean-) | Bağlantı ilk kez yenilenmemişse doğru; aksi takdirde yanlış. |
| [setOdcFile(String value)](#setOdcFile-java.lang.String-) | Bu bağlantının oluşturulduğu dış bağlantı dosyasının tam yolunu belirtir. |
| [setOnlyUseConnectionFile(boolean value)](#setOnlyUseConnectionFile-boolean-) | Bağlantı yenilendiğinde elektronik tablo uygulamasının, odcFile özniteliğiyle belirtilen dış bağlantı dosyasındaki bağlantı bilgilerini her zaman ve yalnızca kullanıp kullanmayacağını gösterir. |
| [setReconnectionMethod(int value)](#setReconnectionMethod-int-) | Bir bağlantı başarısız olduğunda elektronik tablo uygulamasının ne yapması gerektiğini belirtir. |
| [setReconnectionMethodType(int value)](#setReconnectionMethodType-int-) | Bir bağlantı başarısız olduğunda elektronik tablo uygulamasının ne yapması gerektiğini belirtir. |
| [setRefreshInternal(int value)](#setRefreshInternal-int-) | Bağlantının otomatik yenilemeleri arasındaki dakika sayısını belirtir. |
| [setRefreshOnLoad(boolean value)](#setRefreshOnLoad-boolean-) | Dosya açıldığında bu bağlantının yenilenmesi gerekiyorsa doğru; aksi takdirde yanlış. |
| [setSSOId(String value)](#setSSOId-java.lang.String-) | Ara bir spreadsheetML sunucusu ile dış veri kaynağı arasında kimlik doğrulama için kullanılan Tek Oturum Açma (SSO) tanımlayıcısı. |
| [setSaveData(boolean value)](#setSaveData-boolean-) | Bağlantı üzerinden alınan dış verinin bir tabloyu doldurmak için çalışma kitabıyla birlikte kaydedilmesi gerekiyorsa doğru; aksi takdirde yanlış. |
| [setSavePassword(boolean value)](#setSavePassword-boolean-) | Parolanın bağlantı dizesinin bir parçası olarak kaydedilmesi gerekiyorsa doğru; aksi takdirde Yanlış. |
| [setSecondCommand(String value)](#setSecondCommand-java.lang.String-) | PivotTable sunucu tabanlı sayfa alanları kullanıldığında kalıcı olan ikinci komut metni dizesini belirtir. |
| [setSourceFile(String value)](#setSourceFile-java.lang.String-) | Harici veri kaynağı dosya tabanlı olduğunda kullanılır. |
| [setSourceType(int value)](#setSourceType-int-) | Harici bağlantı DataSource türünü ayarlar. |
| [setType(int value)](#setType-int-) | Harici bağlantı DataSource türünü ayarlar. |
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


Döndürür [OLEDBCommandType](../../com.aspose.cells/oledbcommandtype) türü.

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
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isDeleted() {#isDeleted--}
```
public boolean isDeleted()
```


İlgili çalışma kitabı bağlantısının silinip silinmediğini gösterir. Bağlantı silinmişse true; aksi takdirde false.

**Returns:**
boolean
### isNew() {#isNew--}
```
public boolean isNew()
```


Bağlantı ilk kez yenilenmemişse true; aksi takdirde false. Bu durum, kullanıcının sorgu tamamlanmadan dosyayı kaydetmesi durumunda ortaya çıkabilir.

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


Döndürür [OLEDBCommandType](../../com.aspose.cells/oledbcommandtype) türü.

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

