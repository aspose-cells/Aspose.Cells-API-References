---
title: "VbaProject"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет проект VBA."
type: docs
url: /ru/java/com.aspose.cells/vbaproject/
---

**Inheritance:**
java.lang.Object
```
public class VbaProject
```

Представляет проект VBA.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
          // Init VBA project.
         VbaProject vbaProject = workbook.getVbaProject();
         //Saving the Excel file
         workbook.save("book1.xlsm");
```
## Методы

| Метод | Описание |
| --- | --- |
| [copy(VbaProject source)](#copy-com.aspose.cells.VbaProject-) | Скопировать проект VBA из другого файла. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCertRawData()](#getCertRawData--) | Получает необработанные данные сертификата, если этот проект VBA подписан. |
| [getClass()](#getClass--) |  |
| [getEncoding()](#getEncoding--) | Получает кодировку проекта VBA. |
| [getIslockedForViewing()](#getIslockedForViewing--) | Указывает, заблокирован ли этот проект VBA для просмотра. |
| [getModules()](#getModules--) | Получает все объекты [VbaModule](../../com.aspose.cells/vbamodule). |
| [getName()](#getName--) | Получает имя проекта VBA. |
| [getReferences()](#getReferences--) | Получает все ссылки проекта VBA. |
| [hashCode()](#hashCode--) |  |
| [isLockedForView()](#isLockedForView--) | Указывает, заблокирован ли этот проект VBA для просмотра. |
| [isProtected()](#isProtected--) | Указывает, защищён ли этот проект VBA. |
| [isSigned()](#isSigned--) | Указывает, подписан ли VBAcode или нет. |
| [isValidSigned()](#isValidSigned--) | Указывает, действительна ли подпись проекта VBA или нет. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [protect(boolean islockedForViewing, String password)](#protect-boolean-java.lang.String-) | Защищает или снимает защиту с этого проекта VBA. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.cells.Encoding-) | Устанавливает кодировку проекта VBA. |
| [setName(String value)](#setName-java.lang.String-) | Устанавливает имя проекта VBA. |
| [sign(DigitalSignature digitalSignature)](#sign-com.aspose.cells.DigitalSignature-) | Подписать этот проект VBA цифровой подписью |
| [toString()](#toString--) |  |
| [validatePassword(String password)](#validatePassword-java.lang.String-) | Проверяет пароль защиты. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### copy(VbaProject source) {#copy-com.aspose.cells.VbaProject-}
```
public void copy(VbaProject source)
```


Скопировать проект VBA из другого файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| source | [VbaProject](../../com.aspose.cells/vbaproject) |  |

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
### getCertRawData() {#getCertRawData--}
```
public byte[] getCertRawData()
```


Получает необработанные данные сертификата, если этот проект VBA подписан.

**Returns:**
byte[]
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


Получает кодировку проекта VBA.

**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getIslockedForViewing() {#getIslockedForViewing--}
```
public boolean getIslockedForViewing()
```


Указывает, заблокирован ли этот проект VBA для просмотра.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство VbaProject.IsLockedForView. Это свойство будет удалено через 12 месяцев, начиная с июля 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
boolean
### getModules() {#getModules--}
```
public VbaModuleCollection getModules()
```


Получает все объекты [VbaModule](../../com.aspose.cells/vbamodule).

**Returns:**
[VbaModuleCollection](../../com.aspose.cells/vbamodulecollection)
### getName() {#getName--}
```
public String getName()
```


Получает имя проекта VBA.

**Returns:**
java.lang.String
### getReferences() {#getReferences--}
```
public VbaProjectReferenceCollection getReferences()
```


Получает все ссылки проекта VBA.

**Returns:**
[VbaProjectReferenceCollection](../../com.aspose.cells/vbaprojectreferencecollection)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isLockedForView() {#isLockedForView--}
```
public boolean isLockedForView()
```


Указывает, заблокирован ли этот проект VBA для просмотра. Если true, код не будет виден.

**Returns:**
boolean
### isProtected() {#isProtected--}
```
public boolean isProtected()
```


Указывает, защищён ли этот проект VBA.

**Returns:**
boolean
### isSigned() {#isSigned--}
```
public boolean isSigned()
```


Указывает, подписан ли VBAcode или нет.

**Returns:**
boolean
### isValidSigned() {#isValidSigned--}
```
public boolean isValidSigned()
```


Указывает, действительна ли подпись проекта VBA или нет.

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




### protect(boolean islockedForViewing, String password) {#protect-boolean-java.lang.String-}
```
public void protect(boolean islockedForViewing, String password)
```


Защищает или снимает защиту с этого проекта VBA.

**Remarks**

Если islockedForViewing равно true, пароль не может быть null.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| islockedForViewing | boolean | Указывает, блокирует ли проект для просмотра. |
| пароль | java.lang.String | Если значение равно null, снимает защиту с этого проекта VBA, иначе защищает этот проект VBA. |

### setEncoding(Encoding value) {#setEncoding-com.aspose.cells.Encoding-}
```
public void setEncoding(Encoding value)
```


Устанавливает кодировку проекта VBA.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.cells/encoding) |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Устанавливает имя проекта VBA.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### sign(DigitalSignature digitalSignature) {#sign-com.aspose.cells.DigitalSignature-}
```
public void sign(DigitalSignature digitalSignature)
```


Подписать этот проект VBA цифровой подписью

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| digitalSignature | [DigitalSignature](../../com.aspose.cells/digitalsignature) | DigitalSignature |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### validatePassword(String password) {#validatePassword-java.lang.String-}
```
public boolean validatePassword(String password)
```


Проверяет пароль защиты.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| пароль | java.lang.String | пароль |

**Returns:**
логический - Является ли пароль защитным паролем этого проекта VBA
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

