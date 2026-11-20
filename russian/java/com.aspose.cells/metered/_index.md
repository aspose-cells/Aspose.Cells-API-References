---
title: "Metered"
second_title: "Справочник API Aspose.Cells for Java"
description: "Предоставляет методы для установки измеряемого ключа."
type: docs
url: /ru/java/com.aspose.cells/metered/
---

**Inheritance:**
java.lang.Object
```
public class Metered
```

Предоставляет методы для установки измеряемого ключа.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [Metered()](#Metered--) | Инициализирует новый экземпляр этого класса. |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getConsumptionCredit()](#getConsumptionCredit--) | Получает кредит потребления |
| [getConsumptionQuantity()](#getConsumptionQuantity--) | Получает размер файла потребления |
| [getProductName()](#getProductName--) | Получает название продукта |
| [hashCode()](#hashCode--) |  |
| [isMeteredLicensed()](#isMeteredLicensed--) | Проверьте, лицензирована ли metered |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setMeteredKey(String publicKey, String privateKey)](#setMeteredKey-java.lang.String-java.lang.String-) | Устанавливает публичный и приватный ключ metered. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Metered() {#Metered--}
```
public Metered()
```


Инициализирует новый экземпляр этого класса.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getConsumptionCredit() {#getConsumptionCredit--}
```
public static double getConsumptionCredit()
```


Получает кредит потребления

**Returns:**
double - количество потребления
### getConsumptionQuantity() {#getConsumptionQuantity--}
```
public static double getConsumptionQuantity()
```


Получает размер файла потребления

**Returns:**
double - количество потребления
### getProductName() {#getProductName--}
```
public String getProductName()
```


Получает название продукта

**Returns:**
java.lang.String - название продукта
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isMeteredLicensed() {#isMeteredLicensed--}
```
public static boolean isMeteredLicensed()
```


Проверьте, лицензирована ли metered

**Returns:**
boolean - Истина или ложь
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setMeteredKey(String publicKey, String privateKey) {#setMeteredKey-java.lang.String-java.lang.String-}
```
public void setMeteredKey(String publicKey, String privateKey)
```


Устанавливает публичный и приватный ключ metered. Если вы приобретаете лицензию metered, при запуске приложения следует вызвать этот API, обычно этого достаточно. Однако если постоянно не удаётся загрузить данные потребления и проходит более 24 часов, лицензия будет переведена в статус оценки; чтобы избежать такой ситуации, следует регулярно проверять статус лицензии, и если он находится в статусе оценки, вызвать этот API снова.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| publicKey | java.lang.String | публичный ключ |
| privateKey | java.lang.String | приватный ключ |

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
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

