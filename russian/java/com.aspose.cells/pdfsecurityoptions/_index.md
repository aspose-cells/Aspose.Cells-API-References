---
title: "PdfSecurityOptions"
second_title: "Справочник API Aspose.Cells for Java"
description: "Параметры шифрования и прав доступа к PDF‑документу."
type: docs
url: /ru/java/com.aspose.cells/pdfsecurityoptions/
---

**Inheritance:**
java.lang.Object
```
public class PdfSecurityOptions
```

Параметры шифрования и прав доступа для PDF‑документа. PDF/A не допускает настройки безопасности.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [PdfSecurityOptions()](#PdfSecurityOptions--) | Конструктор класса PdfSecurityOptions |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAccessibilityExtractContent()](#getAccessibilityExtractContent--) | Указывает, разрешено ли извлекать текст и графику (в поддержку доступности для пользователей с ограниченными возможностями или для других целей). |
| [getAnnotationsPermission()](#getAnnotationsPermission--) | Указывает, разрешено ли добавлять или изменять текстовые аннотации, заполнять интерактивные поля форм. |
| [getAssembleDocumentPermission()](#getAssembleDocumentPermission--) | Указывает, разрешено ли собирать документ (вставлять, вращать или удалять страницы и создавать закладки или миниатюры), даже если [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) не установлен. |
| [getClass()](#getClass--) |  |
| [getExtractContentPermission()](#getExtractContentPermission--) | Указывает, разрешено ли копировать или иным способом извлекать текст и графику из документа операциями, отличными от контролируемых [getAccessibilityExtractContent()](../../com.aspose.cells/pdfsecurityoptions\#getAccessibilityExtractContent--). |
| [getExtractContentPermissionObsolete()](#getExtractContentPermissionObsolete--) | Разрешение на копирование или извлечение содержимого устарело согласно справочнику PDF. |
| [getFillFormsPermission()](#getFillFormsPermission--) | Указывает, разрешено ли заполнять существующие интерактивные поля форм (включая поля подписи), даже если [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) не установлен. |
| [getFullQualityPrintPermission()](#getFullQualityPrintPermission--) | Указывает, разрешено ли печатать документ в виде представления, из которого можно создать точную цифровую копию содержимого PDF. |
| [getModifyDocumentPermission()](#getModifyDocumentPermission--) | Указывает, разрешено ли изменять содержимое документа операциями, отличными от контролируемых [getAnnotationsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAnnotationsPermission--), [getFillFormsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFillFormsPermission--) и [getAssembleDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAssembleDocumentPermission--). |
| [getOwnerPassword()](#getOwnerPassword--) | Получает пароль владельца зашифрованного PDF‑документа. |
| [getPrintPermission()](#getPrintPermission--) | Указывает, разрешено ли печатать документ. |
| [getUserPassword()](#getUserPassword--) | Получает пользовательский пароль, необходимый для открытия зашифрованного PDF‑документа. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAccessibilityExtractContent(boolean value)](#setAccessibilityExtractContent-boolean-) | Указывает, разрешено ли извлекать текст и графику (в поддержку доступности для пользователей с ограниченными возможностями или для других целей). |
| [setAnnotationsPermission(boolean value)](#setAnnotationsPermission-boolean-) | Указывает, разрешено ли добавлять или изменять текстовые аннотации, заполнять интерактивные поля форм. |
| [setAssembleDocumentPermission(boolean value)](#setAssembleDocumentPermission-boolean-) | Указывает, разрешено ли собирать документ (вставлять, вращать или удалять страницы и создавать закладки или миниатюры), даже если [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) не установлен. |
| [setExtractContentPermission(boolean value)](#setExtractContentPermission-boolean-) | Указывает, разрешено ли копировать или иным способом извлекать текст и графику из документа операциями, отличными от контролируемых [getAccessibilityExtractContent()](../../com.aspose.cells/pdfsecurityoptions\#getAccessibilityExtractContent--). |
| [setExtractContentPermissionObsolete(boolean value)](#setExtractContentPermissionObsolete-boolean-) | Разрешение на копирование или извлечение содержимого устарело согласно справочнику PDF. |
| [setFillFormsPermission(boolean value)](#setFillFormsPermission-boolean-) | Указывает, разрешено ли заполнять существующие интерактивные поля форм (включая поля подписи), даже если [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) не установлен. |
| [setFullQualityPrintPermission(boolean value)](#setFullQualityPrintPermission-boolean-) | Указывает, разрешено ли печатать документ в виде представления, из которого можно создать точную цифровую копию содержимого PDF. |
| [setModifyDocumentPermission(boolean value)](#setModifyDocumentPermission-boolean-) | Указывает, разрешено ли изменять содержимое документа операциями, отличными от контролируемых [getAnnotationsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAnnotationsPermission--), [getFillFormsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFillFormsPermission--) и [getAssembleDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAssembleDocumentPermission--). |
| [setOwnerPassword(String value)](#setOwnerPassword-java.lang.String-) | Устанавливает пароль владельца зашифрованного PDF‑документа. |
| [setPrintPermission(boolean value)](#setPrintPermission-boolean-) | Указывает, разрешено ли печатать документ. |
| [setUserPassword(String value)](#setUserPassword-java.lang.String-) | Устанавливает пользовательский пароль, необходимый для открытия зашифрованного PDF‑документа. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PdfSecurityOptions() {#PdfSecurityOptions--}
```
public PdfSecurityOptions()
```


Конструктор класса PdfSecurityOptions

**Example**

Следующий код устанавливает разрешение печати высокого качества для выходного PDF.

```
         Workbook wb = new Workbook();
         wb.getWorksheets().get(0).getCells().get("A1").setValue("Aspose");
 
         PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
 
 
         PdfSecurityOptions pdfSecurityOptions = new PdfSecurityOptions();
 
         //set owner password
         pdfSecurityOptions.setOwnerPassword("YourOwnerPassword");
 
         //set user password
         pdfSecurityOptions.setUserPassword("YourUserPassword");
 
         //set print permisson
         pdfSecurityOptions.setPrintPermission(true);
 
         //set high resolution for print
         pdfSecurityOptions.setFullQualityPrintPermission(true);
 
 
         pdfSaveOptions.setSecurityOptions(pdfSecurityOptions);
 
         wb.save("output.pdf", pdfSaveOptions);
```

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
### getAccessibilityExtractContent() {#getAccessibilityExtractContent--}
```
public boolean getAccessibilityExtractContent()
```


Указывает, разрешено ли извлекать текст и графику (в поддержку доступности для пользователей с ограниченными возможностями или для других целей).

**Returns:**
boolean
### getAnnotationsPermission() {#getAnnotationsPermission--}
```
public boolean getAnnotationsPermission()
```


Указывает, разрешено ли добавлять или изменять текстовые аннотации, заполнять интерактивные поля форм.

**Remarks**

Если [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) также установлен, создавайте или изменяйте интерактивные поля форм (включая поля подписи).

**Returns:**
boolean
### getAssembleDocumentPermission() {#getAssembleDocumentPermission--}
```
public boolean getAssembleDocumentPermission()
```


Указывает, разрешено ли собирать документ (вставлять, вращать или удалять страницы и создавать закладки или миниатюры), даже если [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) не установлен.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getExtractContentPermission() {#getExtractContentPermission--}
```
public boolean getExtractContentPermission()
```


Указывает, разрешено ли копировать или иным способом извлекать текст и графику из документа операциями, отличными от контролируемых [getAccessibilityExtractContent()](../../com.aspose.cells/pdfsecurityoptions\#getAccessibilityExtractContent--).

**Returns:**
boolean
### getExtractContentPermissionObsolete() {#getExtractContentPermissionObsolete--}
```
public boolean getExtractContentPermissionObsolete()
```


Разрешение на копирование или извлечение содержимого устарело согласно справочнику PDF.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него используйте свойство ExtractContentPermission. Это свойство будет удалено через 12 месяцев, начиная с сентября 2023 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
boolean
### getFillFormsPermission() {#getFillFormsPermission--}
```
public boolean getFillFormsPermission()
```


Указывает, разрешено ли заполнять существующие интерактивные поля форм (включая поля подписи), даже если [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) не установлен.

**Returns:**
boolean
### getFullQualityPrintPermission() {#getFullQualityPrintPermission--}
```
public boolean getFullQualityPrintPermission()
```


Указывает, разрешено ли печатать документ в виде представления, из которого можно создать точную цифровую копию содержимого PDF.

**Remarks**

Когда он не установлен (и [getPrintPermission()](../../com.aspose.cells/pdfsecurityoptions\#getPrintPermission--) установлен), печать ограничивается низкоуровневым представлением внешнего вида, возможно, с ухудшенным качеством.

**Returns:**
boolean
### getModifyDocumentPermission() {#getModifyDocumentPermission--}
```
public boolean getModifyDocumentPermission()
```


Указывает, разрешено ли изменять содержимое документа операциями, отличными от контролируемых [getAnnotationsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAnnotationsPermission--), [getFillFormsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFillFormsPermission--) и [getAssembleDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAssembleDocumentPermission--).

**Returns:**
boolean
### getOwnerPassword() {#getOwnerPassword--}
```
public String getOwnerPassword()
```


Получает пароль владельца зашифрованного PDF‑документа.

**Remarks**

Пароль владельца позволяет пользователю открыть зашифрованный PDF‑документ без каких-либо указанных ограничений доступа.

**Returns:**
java.lang.String
### getPrintPermission() {#getPrintPermission--}
```
public boolean getPrintPermission()
```


Указывает, разрешено ли печатать документ.

**Remarks**

Возможно, не на самом высоком уровне качества, в зависимости от того, установлен ли также [getFullQualityPrintPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFullQualityPrintPermission--).

**Returns:**
boolean
### getUserPassword() {#getUserPassword--}
```
public String getUserPassword()
```


Получает пользовательский пароль, необходимый для открытия зашифрованного PDF‑документа.

**Remarks**

Для просмотра зашифрованного PDF‑документа потребуется пароль владельца или пароль пользователя.

Пароль пользователя может быть null или пустой строкой, в этом случае пароль от пользователя не будет требоваться при открытии PDF‑документа.

Открытие документа с правильным паролем владельца предоставляет полный доступ к документу.

Открытие документа с правильным паролем пользователя (или открытие документа без пароля пользователя) предоставляет ограниченный доступ в соответствии с указанными разрешениями.

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAccessibilityExtractContent(boolean value) {#setAccessibilityExtractContent-boolean-}
```
public void setAccessibilityExtractContent(boolean value)
```


Указывает, разрешено ли извлекать текст и графику (в поддержку доступности для пользователей с ограниченными возможностями или для других целей).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setAnnotationsPermission(boolean value) {#setAnnotationsPermission-boolean-}
```
public void setAnnotationsPermission(boolean value)
```


Указывает, разрешено ли добавлять или изменять текстовые аннотации, заполнять интерактивные поля форм.

**Remarks**

Если [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) также установлен, создавайте или изменяйте интерактивные поля форм (включая поля подписи).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setAssembleDocumentPermission(boolean value) {#setAssembleDocumentPermission-boolean-}
```
public void setAssembleDocumentPermission(boolean value)
```


Указывает, разрешено ли собирать документ (вставлять, вращать или удалять страницы и создавать закладки или миниатюры), даже если [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) не установлен.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setExtractContentPermission(boolean value) {#setExtractContentPermission-boolean-}
```
public void setExtractContentPermission(boolean value)
```


Указывает, разрешено ли копировать или иным способом извлекать текст и графику из документа операциями, отличными от контролируемых [getAccessibilityExtractContent()](../../com.aspose.cells/pdfsecurityoptions\#getAccessibilityExtractContent--).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setExtractContentPermissionObsolete(boolean value) {#setExtractContentPermissionObsolete-boolean-}
```
public void setExtractContentPermissionObsolete(boolean value)
```


Разрешение на копирование или извлечение содержимого устарело согласно справочнику PDF.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него используйте свойство ExtractContentPermission. Это свойство будет удалено через 12 месяцев, начиная с сентября 2023 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setFillFormsPermission(boolean value) {#setFillFormsPermission-boolean-}
```
public void setFillFormsPermission(boolean value)
```


Указывает, разрешено ли заполнять существующие интерактивные поля форм (включая поля подписи), даже если [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) не установлен.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setFullQualityPrintPermission(boolean value) {#setFullQualityPrintPermission-boolean-}
```
public void setFullQualityPrintPermission(boolean value)
```


Указывает, разрешено ли печатать документ в виде представления, из которого можно создать точную цифровую копию содержимого PDF.

**Remarks**

Когда он не установлен (и [getPrintPermission()](../../com.aspose.cells/pdfsecurityoptions\#getPrintPermission--) установлен), печать ограничивается низкоуровневым представлением внешнего вида, возможно, с ухудшенным качеством.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setModifyDocumentPermission(boolean value) {#setModifyDocumentPermission-boolean-}
```
public void setModifyDocumentPermission(boolean value)
```


Указывает, разрешено ли изменять содержимое документа операциями, отличными от контролируемых [getAnnotationsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAnnotationsPermission--), [getFillFormsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFillFormsPermission--) и [getAssembleDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAssembleDocumentPermission--).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setOwnerPassword(String value) {#setOwnerPassword-java.lang.String-}
```
public void setOwnerPassword(String value)
```


Устанавливает пароль владельца зашифрованного PDF‑документа.

**Remarks**

Пароль владельца позволяет пользователю открыть зашифрованный PDF‑документ без каких-либо указанных ограничений доступа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setPrintPermission(boolean value) {#setPrintPermission-boolean-}
```
public void setPrintPermission(boolean value)
```


Указывает, разрешено ли печатать документ.

**Remarks**

Возможно, не на самом высоком уровне качества, в зависимости от того, установлен ли также [getFullQualityPrintPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFullQualityPrintPermission--).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setUserPassword(String value) {#setUserPassword-java.lang.String-}
```
public void setUserPassword(String value)
```


Устанавливает пользовательский пароль, необходимый для открытия зашифрованного PDF‑документа.

**Remarks**

Для просмотра зашифрованного PDF‑документа потребуется пароль владельца или пароль пользователя.

Пароль пользователя может быть null или пустой строкой, в этом случае пароль от пользователя не будет требоваться при открытии PDF‑документа.

Открытие документа с правильным паролем владельца предоставляет полный доступ к документу.

Открытие документа с правильным паролем пользователя (или открытие документа без пароля пользователя) предоставляет ограниченный доступ в соответствии с указанными разрешениями.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

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

