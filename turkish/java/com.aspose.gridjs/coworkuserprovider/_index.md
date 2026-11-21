---
title: "CoWorkUserProvider"
second_title: "Aspose.Cells for Java API Referansı"
description: "İşbirliği modunda kullanıcı sağlayıcı arayüzünü temsil eder. Şu anda yalnızca Java sürümünde mevcuttur, gelecekte .NET/Python sürümünde de bulunacaktır."
type: docs
url: /tr/java/com.aspose.gridjs/coworkuserprovider/
---
```
public interface CoWorkUserProvider
```

İşbirliği modunda kullanıcı sağlayıcı arayüzünü temsil eder. Şu anda yalnızca Java sürümünde mevcuttur, gelecekte .NET/Python sürümünde de bulunacaktır. Müşteri uygulaması bu arayüzü uygulayarak kullanıcı bilgilerini sağlayabilir.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getCurrentUserId()](#getCurrentUserId--) | Mevcut kullanıcının benzersiz tanımlayıcısını alır |
| [getCurrentUserName()](#getCurrentUserName--) | Mevcut kullanıcının kullanıcı adını alır |
| [getPermission()](#getPermission--) | Mevcut kullanıcının izin seviyesini alır |
### getCurrentUserId() {#getCurrentUserId--}
```
public abstract long getCurrentUserId()
```


Mevcut kullanıcının benzersiz tanımlayıcısını alır

**Returns:**
long - Mevcut kullanıcı kimliği
### getCurrentUserName() {#getCurrentUserName--}
```
public abstract String getCurrentUserName()
```


Mevcut kullanıcının kullanıcı adını alır

**Returns:**
java.lang.String - Mevcut kullanıcı adı
### getPermission() {#getPermission--}
```
public abstract int getPermission()
```


Mevcut kullanıcının izin seviyesini alır

**Returns:**
int - [CoWorkUserPermission](../../com.aspose.gridjs/coworkuserpermission). Mevcut kullanıcı izin seviyesi
