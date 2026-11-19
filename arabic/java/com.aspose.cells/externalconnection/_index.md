---
title: "ExternalConnection"
second_title: "Aspose.Cells for Java API Reference"
description: "يحدد اتصال بيانات خارجي"
type: docs
url: /ar/java/com.aspose.cells/externalconnection/
---

**Inheritance:**
java.lang.Object
```
public abstract class ExternalConnection
```

يحدد اتصال بيانات خارجي
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackgroundRefresh()](#getBackgroundRefresh--) | يشير إلى ما إذا كان يمكن تحديث الاتصال في الخلفية (بشكل غير متزامن). |
| [getClass()](#getClass--) |  |
| [getClassType()](#getClassType--) | يحصل على نوع هذا الكائن [ExternalConnection](../../com.aspose.cells/externalconnection). |
| [getCommand()](#getCommand--) | السلسلة التي تحتوي على أمر قاعدة البيانات لتمريره إلى واجهة برمجة تطبيقات موفر البيانات التي ستتفاعل مع المصدر الخارجي لاسترجاع البيانات |
| [getCommandType()](#getCommandType--) | يحدد نوع أمر OLE DB. 1. |
| [getConnectionDescription()](#getConnectionDescription--) | يحدد وصف المستخدم لهذا الاتصال |
| [getConnectionFile()](#getConnectionFile--) | يحصل على ملف الاتصال. |
| [getConnectionId()](#getConnectionId--) | يحدد المعرف الفريد لهذا الاتصال. |
| [getConnectionString()](#getConnectionString--) | يتم استخدام سلسلة معلومات الاتصال للاتصال بمصدر بيانات OLE DB أو ODBC. |
| [getCredentials()](#getCredentials--) | يحدد طريقة المصادقة التي ستُستخدم عند إنشاء (أو إعادة إنشاء) الاتصال. |
| [getCredentialsMethodType()](#getCredentialsMethodType--) | يحدد طريقة المصادقة التي ستُستخدم عند إنشاء (أو إعادة إنشاء) الاتصال. |
| [getId()](#getId--) | يحصل على معرف الاتصال. |
| [getKeepAlive()](#getKeepAlive--) | صحيح عندما يجب على تطبيق جدول البيانات بذل الجهود للحفاظ على الاتصال مفتوحًا. |
| [getName()](#getName--) | يحدد اسم الاتصال. |
| [getOdcFile()](#getOdcFile--) | يحدد المسار الكامل إلى ملف الاتصال الخارجي الذي تم إنشاء هذا الاتصال منه. |
| [getOnlyUseConnectionFile()](#getOnlyUseConnectionFile--) | يشير إلى ما إذا كان يجب على تطبيق جدول البيانات دائمًا وفقط استخدام معلومات الاتصال في ملف الاتصال الخارجي المشار إليه بصفة odcFile عند تحديث الاتصال. |
| [getParameters()](#getParameters--) | يحصل على [ConnectionParameterCollection](../../com.aspose.cells/connectionparametercollection) لاستعلام ODBC أو ويب. |
| [getPowerQueryFormula()](#getPowerQueryFormula--) | يحصل على تعريف صيغة Power Query. |
| [getReconnectionMethod()](#getReconnectionMethod--) | يحدد ما يجب أن يفعله تطبيق جدول البيانات عندما يفشل الاتصال. |
| [getReconnectionMethodType()](#getReconnectionMethodType--) | يحدد ما يجب أن يفعله تطبيق جدول البيانات عندما يفشل الاتصال. |
| [getRefreshInternal()](#getRefreshInternal--) | يحدد عدد الدقائق بين عمليات التحديث التلقائي للاتصال. |
| [getRefreshOnLoad()](#getRefreshOnLoad--) | صحيح إذا كان يجب تحديث هذا الاتصال عند فتح الملف؛ وإلا، خطأ. |
| [getSSOId()](#getSSOId--) | معرف الدخول الأحادي (SSO) المستخدم للمصادقة بين خادم spreadsheetML الوسيط ومصدر البيانات الخارجي. |
| [getSaveData()](#getSaveData--) | صحيح إذا كان يجب حفظ البيانات الخارجية التي تم جلبها عبر الاتصال لتعبئة جدول مع المصنف؛ وإلا، خطأ. |
| [getSavePassword()](#getSavePassword--) | صحيح إذا كان يجب حفظ كلمة المرور كجزء من سلسلة الاتصال؛ وإلا، خطأ. |
| [getSecondCommand()](#getSecondCommand--) | يحدد سلسلة نص الأمر الثانية التي تُحفظ عندما تكون حقول الصفحات المستندة إلى خادم PivotTable قيد الاستخدام. |
| [getSourceFile()](#getSourceFile--) | يُستخدم عندما يكون مصدر البيانات الخارجي قائمًا على ملف. |
| [getSourceType()](#getSourceType--) | يحصل على نوع مصدر البيانات للاتصال الخارجي. |
| [getType()](#getType--) | يحصل على نوع مصدر البيانات للاتصال الخارجي. |
| [hashCode()](#hashCode--) |  |
| [isDeleted()](#isDeleted--) | يشير إلى ما إذا كان اتصال المصنف المرتبط قد تم حذفه. |
| [isNew()](#isNew--) | صحيح إذا لم يتم تحديث الاتصال للمرة الأولى؛ وإلا، خطأ. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackgroundRefresh(boolean value)](#setBackgroundRefresh-boolean-) | يشير إلى ما إذا كان يمكن تحديث الاتصال في الخلفية (بشكل غير متزامن). |
| [setCommand(String value)](#setCommand-java.lang.String-) | السلسلة التي تحتوي على أمر قاعدة البيانات لتمريره إلى واجهة برمجة تطبيقات موفر البيانات التي ستتفاعل مع المصدر الخارجي لاسترجاع البيانات |
| [setCommandType(int value)](#setCommandType-int-) | يحدد نوع أمر OLE DB. 1. |
| [setConnectionDescription(String value)](#setConnectionDescription-java.lang.String-) | يحدد وصف المستخدم لهذا الاتصال |
| [setConnectionString(String value)](#setConnectionString-java.lang.String-) | يتم استخدام سلسلة معلومات الاتصال للاتصال بمصدر بيانات OLE DB أو ODBC. |
| [setCredentials(int value)](#setCredentials-int-) | يحدد طريقة المصادقة التي ستُستخدم عند إنشاء (أو إعادة إنشاء) الاتصال. |
| [setCredentialsMethodType(int value)](#setCredentialsMethodType-int-) | يحدد طريقة المصادقة التي ستُستخدم عند إنشاء (أو إعادة إنشاء) الاتصال. |
| [setDeleted(boolean value)](#setDeleted-boolean-) | يشير إلى ما إذا كان اتصال المصنف المرتبط قد تم حذفه. |
| [setKeepAlive(boolean value)](#setKeepAlive-boolean-) | صحيح عندما يجب على تطبيق جدول البيانات بذل الجهود للحفاظ على الاتصال مفتوحًا. |
| [setName(String value)](#setName-java.lang.String-) | يحدد اسم الاتصال. |
| [setNew(boolean value)](#setNew-boolean-) | صحيح إذا لم يتم تحديث الاتصال للمرة الأولى؛ وإلا، خطأ. |
| [setOdcFile(String value)](#setOdcFile-java.lang.String-) | يحدد المسار الكامل إلى ملف الاتصال الخارجي الذي تم إنشاء هذا الاتصال منه. |
| [setOnlyUseConnectionFile(boolean value)](#setOnlyUseConnectionFile-boolean-) | يشير إلى ما إذا كان يجب على تطبيق جدول البيانات دائمًا وفقط استخدام معلومات الاتصال في ملف الاتصال الخارجي المشار إليه بصفة odcFile عند تحديث الاتصال. |
| [setReconnectionMethod(int value)](#setReconnectionMethod-int-) | يحدد ما يجب أن يفعله تطبيق جدول البيانات عندما يفشل الاتصال. |
| [setReconnectionMethodType(int value)](#setReconnectionMethodType-int-) | يحدد ما يجب أن يفعله تطبيق جدول البيانات عندما يفشل الاتصال. |
| [setRefreshInternal(int value)](#setRefreshInternal-int-) | يحدد عدد الدقائق بين عمليات التحديث التلقائي للاتصال. |
| [setRefreshOnLoad(boolean value)](#setRefreshOnLoad-boolean-) | صحيح إذا كان يجب تحديث هذا الاتصال عند فتح الملف؛ وإلا، خطأ. |
| [setSSOId(String value)](#setSSOId-java.lang.String-) | معرف الدخول الأحادي (SSO) المستخدم للمصادقة بين خادم spreadsheetML الوسيط ومصدر البيانات الخارجي. |
| [setSaveData(boolean value)](#setSaveData-boolean-) | صحيح إذا كان يجب حفظ البيانات الخارجية التي تم جلبها عبر الاتصال لتعبئة جدول مع المصنف؛ وإلا، خطأ. |
| [setSavePassword(boolean value)](#setSavePassword-boolean-) | صحيح إذا كان يجب حفظ كلمة المرور كجزء من سلسلة الاتصال؛ وإلا، خطأ. |
| [setSecondCommand(String value)](#setSecondCommand-java.lang.String-) | يحدد سلسلة نص الأمر الثانية التي تُحفظ عندما تكون حقول الصفحات المستندة إلى خادم PivotTable قيد الاستخدام. |
| [setSourceFile(String value)](#setSourceFile-java.lang.String-) | يُستخدم عندما يكون مصدر البيانات الخارجي قائمًا على ملف. |
| [setSourceType(int value)](#setSourceType-int-) | يضبط نوع مصدر البيانات للاتصال الخارجي. |
| [setType(int value)](#setType-int-) | يضبط نوع مصدر البيانات للاتصال الخارجي. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getBackgroundRefresh() {#getBackgroundRefresh--}
```
public boolean getBackgroundRefresh()
```


يشير إلى ما إذا كان يمكن تحديث الاتصال في الخلفية (بشكل غير متزامن). true إذا كان الاستخدام المفضل للاتصال هو التحديث غير المتزامن في الخلفية؛ false إذا كان الاستخدام المفضل للاتصال هو التحديث المتزامن في الواجهة الأمامية.

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
public abstract int getClassType()
```


يحصل على نوع هذا الكائن [ExternalConnection](../../com.aspose.cells/externalconnection).

انظر [ExternalConnectionClassType](../../com.aspose.cells/externalconnectionclasstype).

**Returns:**
int
### getCommand() {#getCommand--}
```
public String getCommand()
```


السلسلة التي تحتوي على أمر قاعدة البيانات لتمريره إلى واجهة برمجة تطبيقات موفر البيانات التي ستتفاعل مع المصدر الخارجي لاسترجاع البيانات

**Returns:**
java.lang.String
### getCommandType() {#getCommandType--}
```
public int getCommandType()
```


يحدد نوع أمر OLE DB. 1. تحدد الاستعلام اسم المكعب 2. تحدد الاستعلام بيان SQL 3. تحدد الاستعلام اسم جدول 4. تحدد الاستعلام أن المعلومات الافتراضية قد تم تقديمها، ويعتمد على الموفر كيفية تفسيرها. 5. الاستعلام يكون ضد موفر بيانات قائمة على الويب.

انظر [OLEDBCommandType](../../com.aspose.cells/oledbcommandtype).

**Returns:**
int
### getConnectionDescription() {#getConnectionDescription--}
```
public String getConnectionDescription()
```


يحدد وصف المستخدم لهذا الاتصال

**Returns:**
java.lang.String
### getConnectionFile() {#getConnectionFile--}
```
public String getConnectionFile()
```


يحصل على ملف الاتصال.

**Returns:**
java.lang.String
### getConnectionId() {#getConnectionId--}
```
public int getConnectionId()
```


يحدد المعرف الفريد لهذا الاتصال.

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية ExternalConnection.Id. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ أكتوبر 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
int
### getConnectionString() {#getConnectionString--}
```
public String getConnectionString()
```


يتم استخدام سلسلة معلومات الاتصال للاتصال بمصدر بيانات OLE DB أو ODBC.

**Returns:**
java.lang.String
### getCredentials() {#getCredentials--}
```
public int getCredentials()
```


يحدد طريقة المصادقة التي ستُستخدم عند إنشاء (أو إعادة إنشاء) الاتصال.

انظر [CredentialsMethodType](../../com.aspose.cells/credentialsmethodtype).

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية ExternalConnection.CredentialsMethodType. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ أكتوبر 2017. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
int
### getCredentialsMethodType() {#getCredentialsMethodType--}
```
public int getCredentialsMethodType()
```


يحدد طريقة المصادقة التي ستُستخدم عند إنشاء (أو إعادة إنشاء) الاتصال.

انظر [CredentialsMethodType](../../com.aspose.cells/credentialsmethodtype).

**Returns:**
int
### getId() {#getId--}
```
public int getId()
```


يحصل على معرف الاتصال.

**Returns:**
int
### getKeepAlive() {#getKeepAlive--}
```
public boolean getKeepAlive()
```


صحيح عندما يجب على تطبيق الجداول الإلكترونية بذل الجهد للحفاظ على الاتصال مفتوحًا. عندما يكون خطأ، يجب على التطبيق إغلاق الاتصال بعد استرجاع المعلومات.

**Returns:**
boolean
### getName() {#getName--}
```
public String getName()
```


يحدد اسم الاتصال. يجب أن يكون لكل اتصال اسم فريد.

**Returns:**
java.lang.String
### getOdcFile() {#getOdcFile--}
```
public String getOdcFile()
```


يحدد المسار الكامل إلى ملف الاتصال الخارجي الذي تم إنشاء هذا الاتصال منه. إذا فشل الاتصال أثناء محاولة تحديث البيانات، وكان reconnectionMethod=1، فستحاول تطبيق الجداول الإلكترونية مرة أخرى باستخدام المعلومات من ملف الاتصال الخارجي بدلاً من كائن الاتصال المضمن داخل المصنف.

**Returns:**
java.lang.String
### getOnlyUseConnectionFile() {#getOnlyUseConnectionFile--}
```
public boolean getOnlyUseConnectionFile()
```


يشير إلى ما إذا كان يجب على تطبيق الجداول الإلكترونية دائمًا وفقط استخدام معلومات الاتصال في ملف الاتصال الخارجي المشار إليه بصفة odcFile عند تحديث الاتصال. إذا كان خطأ، يجب على تطبيق الجداول الإلكترونية اتباع الإجراء المشار إليه بصفة reconnectionMethod.

**Returns:**
boolean
### getParameters() {#getParameters--}
```
public ConnectionParameterCollection getParameters()
```


يحصل على [ConnectionParameterCollection](../../com.aspose.cells/connectionparametercollection) لاستعلام ODBC أو ويب.

**Returns:**
[ConnectionParameterCollection](../../com.aspose.cells/connectionparametercollection)
### getPowerQueryFormula() {#getPowerQueryFormula--}
```
public PowerQueryFormula getPowerQueryFormula()
```


يحصل على تعريف صيغة Power Query.

**Returns:**
[PowerQueryFormula](../../com.aspose.cells/powerqueryformula)
### getReconnectionMethod() {#getReconnectionMethod--}
```
public int getReconnectionMethod()
```


يحدد ما يجب على تطبيق الجداول الإلكترونية القيام به عندما يفشل الاتصال. القيمة الافتراضية هي ReConnectionMethodType.Required.

انظر [ReConnectionMethodType](../../com.aspose.cells/reconnectionmethodtype).

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية ExternalConnection.ReconnectionMethodType. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ أكتوبر 2017. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
int
### getReconnectionMethodType() {#getReconnectionMethodType--}
```
public int getReconnectionMethodType()
```


يحدد ما يجب على تطبيق الجداول الإلكترونية القيام به عندما يفشل الاتصال. القيمة الافتراضية هي ReConnectionMethodType.Required.

انظر [ReConnectionMethodType](../../com.aspose.cells/reconnectionmethodtype).

**Returns:**
int
### getRefreshInternal() {#getRefreshInternal--}
```
public int getRefreshInternal()
```


يحدد عدد الدقائق بين عمليات التحديث التلقائي للاتصال.

**Returns:**
int
### getRefreshOnLoad() {#getRefreshOnLoad--}
```
public boolean getRefreshOnLoad()
```


صحيح إذا كان يجب تحديث هذا الاتصال عند فتح الملف؛ وإلا، خطأ.

**Returns:**
boolean
### getSSOId() {#getSSOId--}
```
public String getSSOId()
```


معرف الدخول الأحادي (SSO) المستخدم للمصادقة بين خادم spreadsheetML الوسيط ومصدر البيانات الخارجي.

**Returns:**
java.lang.String
### getSaveData() {#getSaveData--}
```
public boolean getSaveData()
```


صحيح إذا كان يجب حفظ البيانات الخارجية التي تم جلبها عبر الاتصال لتعبئة جدول مع المصنف؛ وإلا، خطأ.

**Returns:**
boolean
### getSavePassword() {#getSavePassword--}
```
public boolean getSavePassword()
```


صحيح إذا كان يجب حفظ كلمة المرور كجزء من سلسلة الاتصال؛ وإلا، خطأ.

**Returns:**
boolean
### getSecondCommand() {#getSecondCommand--}
```
public String getSecondCommand()
```


يحدد سلسلة نص أمر ثانية تُحفظ عندما تكون حقول الصفحات المستندة إلى الخادم في PivotTable قيد الاستخدام. بالنسبة لاتصالات ODBC، عادةً ما يكون serverCommand استعلامًا أوسع من command (لا توجد جملة WHERE في الأول). استنادًا إلى هذين الأمرين (Command و ServerCommand)، يمكن ملء واجهة المستخدم للمعلمات وإنشاء استعلامات معلمة.

**Returns:**
java.lang.String
### getSourceFile() {#getSourceFile--}
```
public String getSourceFile()
```


يُستخدم عندما يكون مصدر البيانات الخارجي قائمًا على ملف. عندما يفشل الاتصال بمثل هذا المصدر، يحاول تطبيق الجداول الإلكترونية الاتصال مباشرةً بهذا الملف. قد يُعبّر عنه في صيغة URI أو بنظام مسار ملف خاص بالنظام.

**Returns:**
java.lang.String
### getSourceType() {#getSourceType--}
```
public int getSourceType()
```


يحصل على نوع مصدر البيانات للاتصال الخارجي.

انظر [ConnectionDataSourceType](../../com.aspose.cells/connectiondatasourcetype).

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


يحصل على نوع مصدر البيانات للاتصال الخارجي.

انظر [ConnectionDataSourceType](../../com.aspose.cells/connectiondatasourcetype).

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية ExternalConnection.SourceType. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ أكتوبر 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

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


يشير إلى ما إذا كان اتصال المصنف المرتبط قد تم حذفه. true إذا تم حذف الاتصال؛ وإلا false.

**Returns:**
boolean
### isNew() {#isNew--}
```
public boolean isNew()
```


true إذا لم يتم تحديث الاتصال للمرة الأولى؛ وإلا false. قد يحدث هذا الوضع عندما يقوم المستخدم بحفظ الملف قبل أن تنتهي الاستعلام من الإرجاع.

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


يشير إلى ما إذا كان يمكن تحديث الاتصال في الخلفية (بشكل غير متزامن). true إذا كان الاستخدام المفضل للاتصال هو التحديث غير المتزامن في الخلفية؛ false إذا كان الاستخدام المفضل للاتصال هو التحديث المتزامن في الواجهة الأمامية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setCommand(String value) {#setCommand-java.lang.String-}
```
public void setCommand(String value)
```


السلسلة التي تحتوي على أمر قاعدة البيانات لتمريره إلى واجهة برمجة تطبيقات موفر البيانات التي ستتفاعل مع المصدر الخارجي لاسترجاع البيانات

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setCommandType(int value) {#setCommandType-int-}
```
public void setCommandType(int value)
```


يحدد نوع أمر OLE DB. 1. تحدد الاستعلام اسم المكعب 2. تحدد الاستعلام بيان SQL 3. تحدد الاستعلام اسم جدول 4. تحدد الاستعلام أن المعلومات الافتراضية قد تم تقديمها، ويعتمد على الموفر كيفية تفسيرها. 5. الاستعلام يكون ضد موفر بيانات قائمة على الويب.

انظر [OLEDBCommandType](../../com.aspose.cells/oledbcommandtype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setConnectionDescription(String value) {#setConnectionDescription-java.lang.String-}
```
public void setConnectionDescription(String value)
```


يحدد وصف المستخدم لهذا الاتصال

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setConnectionString(String value) {#setConnectionString-java.lang.String-}
```
public void setConnectionString(String value)
```


يتم استخدام سلسلة معلومات الاتصال للاتصال بمصدر بيانات OLE DB أو ODBC.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setCredentials(int value) {#setCredentials-int-}
```
public void setCredentials(int value)
```


يحدد طريقة المصادقة التي ستُستخدم عند إنشاء (أو إعادة إنشاء) الاتصال.

انظر [CredentialsMethodType](../../com.aspose.cells/credentialsmethodtype).

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية ExternalConnection.CredentialsMethodType. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ أكتوبر 2017. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setCredentialsMethodType(int value) {#setCredentialsMethodType-int-}
```
public void setCredentialsMethodType(int value)
```


يحدد طريقة المصادقة التي ستُستخدم عند إنشاء (أو إعادة إنشاء) الاتصال.

انظر [CredentialsMethodType](../../com.aspose.cells/credentialsmethodtype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setDeleted(boolean value) {#setDeleted-boolean-}
```
public void setDeleted(boolean value)
```


يشير إلى ما إذا كان اتصال المصنف المرتبط قد تم حذفه. true إذا تم حذف الاتصال؛ وإلا false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setKeepAlive(boolean value) {#setKeepAlive-boolean-}
```
public void setKeepAlive(boolean value)
```


صحيح عندما يجب على تطبيق الجداول الإلكترونية بذل الجهد للحفاظ على الاتصال مفتوحًا. عندما يكون خطأ، يجب على التطبيق إغلاق الاتصال بعد استرجاع المعلومات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


يحدد اسم الاتصال. يجب أن يكون لكل اتصال اسم فريد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setNew(boolean value) {#setNew-boolean-}
```
public void setNew(boolean value)
```


true إذا لم يتم تحديث الاتصال للمرة الأولى؛ وإلا false. قد يحدث هذا الوضع عندما يقوم المستخدم بحفظ الملف قبل أن تنتهي الاستعلام من الإرجاع.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setOdcFile(String value) {#setOdcFile-java.lang.String-}
```
public void setOdcFile(String value)
```


يحدد المسار الكامل إلى ملف الاتصال الخارجي الذي تم إنشاء هذا الاتصال منه. إذا فشل الاتصال أثناء محاولة تحديث البيانات، وكان reconnectionMethod=1، فستحاول تطبيق الجداول الإلكترونية مرة أخرى باستخدام المعلومات من ملف الاتصال الخارجي بدلاً من كائن الاتصال المضمن داخل المصنف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setOnlyUseConnectionFile(boolean value) {#setOnlyUseConnectionFile-boolean-}
```
public void setOnlyUseConnectionFile(boolean value)
```


يشير إلى ما إذا كان يجب على تطبيق الجداول الإلكترونية دائمًا وفقط استخدام معلومات الاتصال في ملف الاتصال الخارجي المشار إليه بصفة odcFile عند تحديث الاتصال. إذا كان خطأ، يجب على تطبيق الجداول الإلكترونية اتباع الإجراء المشار إليه بصفة reconnectionMethod.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setReconnectionMethod(int value) {#setReconnectionMethod-int-}
```
public void setReconnectionMethod(int value)
```


يحدد ما يجب على تطبيق الجداول الإلكترونية القيام به عندما يفشل الاتصال. القيمة الافتراضية هي ReConnectionMethodType.Required.

انظر [ReConnectionMethodType](../../com.aspose.cells/reconnectionmethodtype).

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية ExternalConnection.ReconnectionMethodType. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ أكتوبر 2017. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setReconnectionMethodType(int value) {#setReconnectionMethodType-int-}
```
public void setReconnectionMethodType(int value)
```


يحدد ما يجب على تطبيق الجداول الإلكترونية القيام به عندما يفشل الاتصال. القيمة الافتراضية هي ReConnectionMethodType.Required.

انظر [ReConnectionMethodType](../../com.aspose.cells/reconnectionmethodtype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setRefreshInternal(int value) {#setRefreshInternal-int-}
```
public void setRefreshInternal(int value)
```


يحدد عدد الدقائق بين عمليات التحديث التلقائي للاتصال.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setRefreshOnLoad(boolean value) {#setRefreshOnLoad-boolean-}
```
public void setRefreshOnLoad(boolean value)
```


صحيح إذا كان يجب تحديث هذا الاتصال عند فتح الملف؛ وإلا، خطأ.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setSSOId(String value) {#setSSOId-java.lang.String-}
```
public void setSSOId(String value)
```


معرف الدخول الأحادي (SSO) المستخدم للمصادقة بين خادم spreadsheetML الوسيط ومصدر البيانات الخارجي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setSaveData(boolean value) {#setSaveData-boolean-}
```
public void setSaveData(boolean value)
```


صحيح إذا كان يجب حفظ البيانات الخارجية التي تم جلبها عبر الاتصال لتعبئة جدول مع المصنف؛ وإلا، خطأ.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setSavePassword(boolean value) {#setSavePassword-boolean-}
```
public void setSavePassword(boolean value)
```


صحيح إذا كان يجب حفظ كلمة المرور كجزء من سلسلة الاتصال؛ وإلا، خطأ.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setSecondCommand(String value) {#setSecondCommand-java.lang.String-}
```
public void setSecondCommand(String value)
```


يحدد سلسلة نص أمر ثانية تُحفظ عندما تكون حقول الصفحات المستندة إلى الخادم في PivotTable قيد الاستخدام. بالنسبة لاتصالات ODBC، عادةً ما يكون serverCommand استعلامًا أوسع من command (لا توجد جملة WHERE في الأول). استنادًا إلى هذين الأمرين (Command و ServerCommand)، يمكن ملء واجهة المستخدم للمعلمات وإنشاء استعلامات معلمة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setSourceFile(String value) {#setSourceFile-java.lang.String-}
```
public void setSourceFile(String value)
```


يُستخدم عندما يكون مصدر البيانات الخارجي قائمًا على ملف. عندما يفشل الاتصال بمثل هذا المصدر، يحاول تطبيق الجداول الإلكترونية الاتصال مباشرةً بهذا الملف. قد يُعبّر عنه في صيغة URI أو بنظام مسار ملف خاص بالنظام.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setSourceType(int value) {#setSourceType-int-}
```
public void setSourceType(int value)
```


يضبط نوع مصدر البيانات للاتصال الخارجي.

انظر [ConnectionDataSourceType](../../com.aspose.cells/connectiondatasourcetype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


يضبط نوع مصدر البيانات للاتصال الخارجي.

انظر [ConnectionDataSourceType](../../com.aspose.cells/connectiondatasourcetype).

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية ExternalConnection.SourceType. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ أكتوبر 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

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
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

