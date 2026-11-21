---
title: "GridJsLogger"
second_title: "Aspose.Cells for Java API Referansı"
description: "GridJs sunucusu için hafif bir günlükleme sistemi sağlar."
type: docs
url: /tr/java/com.aspose.gridjs/gridjslogger/
---

**Inheritance:**
java.lang.Object
```
public class GridJsLogger
```

GridJs sunucusu için hafif bir günlükleme sistemi sağlar. Yapılandırılabilir günlük seviyeleriyle konsol ve dosya çıktısını destekler. Varsayılan seviye Yok'tur. DEBUG derlemesinde, varsayılan seviye Debug'dir (tüm mesajları çıktılar). Günlük dosyası kaydırmayı gün/hafta/ay bazında destekler.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [closeLogFile()](#closeLogFile--) | Günlük dosyası yazarını kapatır ve dosya çıktısını devre dışı bırakır. |
| [debug(String message)](#debug-java.lang.String-) | Debug seviyesinde bir mesaj kaydeder. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [error(String message)](#error-java.lang.String-) | Error seviyesinde bir mesaj kaydeder. |
| [getClass()](#getClass--) |  |
| [getEnableConsoleOutput()](#getEnableConsoleOutput--) | Günlük mesajlarının konsola çıktılanıp çıktılanmayacağını alır. |
| [getEnableFileOutput()](#getEnableFileOutput--) | Günlük mesajlarının bir dosyaya çıktılanıp çıktılanmayacağını alır. |
| [getLevel()](#getLevel--) | Minimum günlük seviyesini alır. |
| [getLogFilePath()](#getLogFilePath--) | Mevcut günlük dosyası yolunu alır, ayarlanmamışsa null döner. |
| [getMaxFileSize()](#getMaxFileSize--) | Kaydırma öncesi tek bir günlük dosyasının maksimum boyutunu (bayt cinsinden) alır. |
| [hashCode()](#hashCode--) |  |
| [info(String message)](#info-java.lang.String-) | Info seviyesinde bir mesaj kaydeder. |
| [log(int level, String message)](#log-int-java.lang.String-) | Belirtilen seviyede bir mesaj kaydeder. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setEnableConsoleOutput(boolean value)](#setEnableConsoleOutput-boolean-) | Günlük mesajlarını konsola çıkarmayı ayarlar. |
| [setEnableFileOutput(boolean value)](#setEnableFileOutput-boolean-) | Günlük mesajlarını bir dosyaya çıkarmayı ayarlar. |
| [setLevel(int value)](#setLevel-int-) | Minimum günlük seviyesini ayarlar. |
| [setLogDirectory(String directory)](#setLogDirectory-java.lang.String-) | Günlük dizinini günlük dönen dosya stratejisiyle ayarlar ve dosya çıktısını etkinleştirir. |
| [setLogDirectory(String directory, int rolling)](#setLogDirectory-java.lang.String-int-) | Günlük dizinini dönen dosya stratejisiyle ayarlar ve dosya çıktısını etkinleştirir. |
| [setLogDirectory(String directory, int rolling, String filePrefix)](#setLogDirectory-java.lang.String-int-java.lang.String-) | Günlük dizinini dönen dosya stratejisiyle ayarlar ve dosya çıktısını etkinleştirir. |
| [setLogFile(String filePath)](#setLogFile-java.lang.String-) | Günlük dosyası yolunu ayarlar ve dosya çıktısını etkinleştirir (tek dosya modu, döndürme yok). |
| [setLogFile(String filePath, boolean append)](#setLogFile-java.lang.String-boolean-) | Günlük dosyası yolunu ayarlar ve dosya çıktısını etkinleştirir (tek dosya modu, döndürme yok). |
| [setMaxFileSize(long value)](#setMaxFileSize-long-) | Dönen öncesinde tek bir günlük dosyasının maksimum boyutunu (bayt cinsinden) ayarlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
| [warn(String message)](#warn-java.lang.String-) | Uyarı seviyesinde bir mesaj kaydeder. |
### closeLogFile() {#closeLogFile--}
```
public static void closeLogFile()
```


Günlük dosyası yazarını kapatır ve dosya çıktısını devre dışı bırakır.

### debug(String message) {#debug-java.lang.String-}
```
public static void debug(String message)
```


Debug seviyesinde bir mesaj kaydeder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| mesaj | java.lang.String |  |

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
### error(String message) {#error-java.lang.String-}
```
public static void error(String message)
```


Error seviyesinde bir mesaj kaydeder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| mesaj | java.lang.String |  |

### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getEnableConsoleOutput() {#getEnableConsoleOutput--}
```
public static boolean getEnableConsoleOutput()
```


Günlük mesajlarını konsola çıkarmayı alır. Varsayılan false'tur.

**Returns:**
boolean
### getEnableFileOutput() {#getEnableFileOutput--}
```
public static boolean getEnableFileOutput()
```


Günlük mesajlarını bir dosyaya çıkarmayı alır. Varsayılan false'tur. Etkinleştirmeden önce [setLogFile(String)](../../com.aspose.gridjs/gridjslogger\#setLogFile-String-) veya [setLogDirectory(String)](../../com.aspose.gridjs/gridjslogger\#setLogDirectory-String-) çağırmalısınız.

**Returns:**
boolean
### getLevel() {#getLevel--}
```
public static int getLevel()
```


Minimum günlük seviyesini alır. Bu seviyenin altındaki mesajlar yok sayılır. Varsayılan None'dur.

Bakınız [GridJsLogLevel](../../com.aspose.gridjs/gridjsloglevel).

**Returns:**
int
### getLogFilePath() {#getLogFilePath--}
```
public static String getLogFilePath()
```


Mevcut günlük dosyası yolunu alır, ayarlanmamışsa null döner.

**Returns:**
java.lang.String
### getMaxFileSize() {#getMaxFileSize--}
```
public static long getMaxFileSize()
```


Dönen öncesinde tek bir günlük dosyasının maksimum boyutunu (bayt cinsinden) alır. Yalnızca döndürme etkin olduğunda geçerlidir. 0, boyut sınırlaması olmadığı anlamına gelir. Varsayılan 0'dır.

**Returns:**
long
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### info(String message) {#info-java.lang.String-}
```
public static void info(String message)
```


Info seviyesinde bir mesaj kaydeder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| mesaj | java.lang.String |  |

### log(int level, String message) {#log-int-java.lang.String-}
```
public static void log(int level, String message)
```


Belirtilen seviyede bir mesaj kaydeder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| level | int | [GridJsLogLevel](../../com.aspose.gridjs/gridjsloglevel). Günlük seviyesi. |
| mesaj | java.lang.String | Kaydedilecek mesaj. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setEnableConsoleOutput(boolean value) {#setEnableConsoleOutput-boolean-}
```
public static void setEnableConsoleOutput(boolean value)
```


Günlük mesajlarını konsola çıkarmayı ayarlar. Varsayılan false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setEnableFileOutput(boolean value) {#setEnableFileOutput-boolean-}
```
public static void setEnableFileOutput(boolean value)
```


Günlük mesajlarını bir dosyaya çıkarmayı ayarlar. Varsayılan false'tur. Etkinleştirmeden önce [setLogFile(String)](../../com.aspose.gridjs/gridjslogger\#setLogFile-String-) veya [setLogDirectory(String)](../../com.aspose.gridjs/gridjslogger\#setLogDirectory-String-) çağırmalısınız.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setLevel(int value) {#setLevel-int-}
```
public static void setLevel(int value)
```


Minimum günlük seviyesini ayarlar. Bu seviyenin altındaki mesajlar yok sayılır. Varsayılan None'dur.

Bakınız [GridJsLogLevel](../../com.aspose.gridjs/gridjsloglevel).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setLogDirectory(String directory) {#setLogDirectory-java.lang.String-}
```
public static void setLogDirectory(String directory)
```


Günlük dizinini günlük dönen dosya stratejisiyle ayarlar ve dosya çıktısını etkinleştirir. Günlük dosyaları şu şekilde adlandırılır: gridjs\_\{period\}.log

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | java.lang.String | Günlük dosyalarını depolamak için dizin. |

### setLogDirectory(String directory, int rolling) {#setLogDirectory-java.lang.String-int-}
```
public static void setLogDirectory(String directory, int rolling)
```


Günlük dizinini dönen dosya stratejisiyle ayarlar ve dosya çıktısını etkinleştirir. Günlük dosyaları şu şekilde adlandırılır: gridjs\_\{period\}.log

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | java.lang.String | Günlük dosyalarını depolamak için dizin. |
| rolling | int | [GridJsLogRolling](../../com.aspose.gridjs/gridjslogrolling). Döndürme stratejisi (Günlük/Haftalık/Aylık). |

### setLogDirectory(String directory, int rolling, String filePrefix) {#setLogDirectory-java.lang.String-int-java.lang.String-}
```
public static void setLogDirectory(String directory, int rolling, String filePrefix)
```


Günlük dizinini dönen dosya stratejisiyle ayarlar ve dosya çıktısını etkinleştirir. Günlük dosyaları şu şekilde adlandırılır: \{prefix\}\_\{period\}.log Örnekler: gridjs\_2026-07-27.log (Günlük), gridjs\_2026-W30.log (Haftalık), gridjs\_2026-07.log (Aylık)

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | java.lang.String | Günlük dosyalarını depolamak için dizin. |
| rolling | int | [GridJsLogRolling](../../com.aspose.gridjs/gridjslogrolling). Döndürme stratejisi (Günlük/Haftalık/Aylık). |
| filePrefix | java.lang.String | Dosya adı öneki. |

### setLogFile(String filePath) {#setLogFile-java.lang.String-}
```
public static void setLogFile(String filePath)
```


Günlük dosyası yolunu ayarlar ve dosya çıktısını etkinleştirir (tek dosya modu, döndürme yok). Mevcut dosyaya ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| filePath | java.lang.String | Günlük dosyasının tam yolu. |

### setLogFile(String filePath, boolean append) {#setLogFile-java.lang.String-boolean-}
```
public static void setLogFile(String filePath, boolean append)
```


Günlük dosyası yolunu ayarlar ve dosya çıktısını etkinleştirir (tek dosya modu, döndürme yok).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| filePath | java.lang.String | Günlük dosyasının tam yolu. |
| ekle | boolean | Mevcut dosyaya eklenip eklenmeyeceği. |

### setMaxFileSize(long value) {#setMaxFileSize-long-}
```
public static void setMaxFileSize(long value)
```


Döndürmeden önce tek bir günlük dosyasının maksimum boyutunu (bayt cinsinden) ayarlar. Yalnızca döndürme etkin olduğunda etkilidir. 0, boyut sınırlaması olmadığı anlamına gelir. Varsayılan değer 0'dır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | long |  |

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

### warn(String message) {#warn-java.lang.String-}
```
public static void warn(String message)
```


Uyarı seviyesinde bir mesaj kaydeder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| mesaj | java.lang.String |  |

