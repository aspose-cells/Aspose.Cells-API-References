---
title: DBConnection
second_title: Aspose.Cells لمرجع .NET API
description: تحديد كافة الخصائص المقترنة باتصال بيانات خارجي ODBC أو OLE DB.
type: docs
weight: 3280
url: /ar/net/aspose.cells.externalconnections/dbconnection/
---
## DBConnection class

تحديد كافة الخصائص المقترنة باتصال بيانات خارجي ODBC أو OLE DB.

```csharp
public class DBConnection : ExternalConnection
```

## الخصائص

| اسم | وصف |
| --- | --- |
| [BackgroundRefresh](../../aspose.cells.externalconnections/externalconnection/backgroundrefresh) { get; set; } | يشير إلى ما إذا كان يمكن تحديث الاتصال في الخلفية (بشكل غير متزامن). true إذا كان الاستخدام المفضل للاتصال هو التحديث غير المتزامن في الخلفية ؛ خطأ إذا كان الاستخدام المفضل للاتصال هو التحديث المتزامن في المقدمة. |
| [Command](../../aspose.cells.externalconnections/dbconnection/command) { get; set; } | السلسلة التي تحتوي على أمر قاعدة البيانات لتمريرها إلى واجهة برمجة تطبيقات موفر البيانات والتي ستتفاعل مع المصدر الخارجي لاسترداد data |
| [CommandType](../../aspose.cells.externalconnections/dbconnection/commandtype) { get; set; } | يحدد نوع أمر OLE DB. 1. يحدد الاستعلام اسم مكعب 2. يحدد الاستعلام جملة SQL 3. يحدد الاستعلام اسم جدول 4. يحدد الاستعلام أن المعلومات الافتراضية قد تم تقديمها ، والأمر متروك للموفر لكيفية التفسير. 5. الاستعلام ضد مزود بيانات قائمة على الويب. |
| [ConnectionDescription](../../aspose.cells.externalconnections/externalconnection/connectiondescription) { get; set; } | تحديد وصف المستخدم لهذا الاتصال |
| [ConnectionId](../../aspose.cells.externalconnections/externalconnection/connectionid) { get; } | يحدد المعرف الفريد لهذا الاتصال. |
| [ConnectionInfo](../../aspose.cells.externalconnections/dbconnection/connectioninfo) { get; set; } | يتم استخدام سلسلة معلومات الاتصال لإجراء اتصال بمصدر بيانات OLE DB أو ODBC. |
| [CredentialsMethodType](../../aspose.cells.externalconnections/externalconnection/credentialsmethodtype) { get; set; } | يحدد طريقة المصادقة التي سيتم استخدامها عند إنشاء (أو إعادة تأسيس) الاتصال . |
| [Id](../../aspose.cells.externalconnections/externalconnection/id) { get; } | يحصل على معرف الاتصال. |
| [IsDeleted](../../aspose.cells.externalconnections/externalconnection/isdeleted) { get; set; } | يشير إلى ما إذا كان قد تم حذف اتصال المصنف المرتبط. صحيح إذا تم حذف الاتصال ؛ وإلا ، خطأ . |
| [IsNew](../../aspose.cells.externalconnections/externalconnection/isnew) { get; set; } | True إذا لم يتم تحديث الاتصال لأول مرة ؛ خلاف ذلك ، خطأ. يمكن أن تحدث هذه الحالة عندما يحفظ المستخدم الملف قبل انتهاء استعلام العودة. |
| [KeepAlive](../../aspose.cells.externalconnections/externalconnection/keepalive) { get; set; } | يكون هذا صحيحًا عندما يجب أن يبذل تطبيق جدول البيانات جهودًا لإبقاء الاتصال مفتوحًا. عندما يكون خطأ ، يجب أن يغلق التطبيق الاتصال بعد استرداد معلومات . |
| [Name](../../aspose.cells.externalconnections/externalconnection/name) { get; set; } | يحدد اسم الاتصال. يجب أن يكون لكل اتصال اسم فريد. |
| [OdcFile](../../aspose.cells.externalconnections/externalconnection/odcfile) { get; set; } | يحدد المسار الكامل لملف الاتصال الخارجي الذي تم إنشاء هذا الاتصال منه. إذا فشل الاتصال أثناء محاولة تحديث البيانات ، وطريقة إعادة الاتصال = 1 ، فسيحاول تطبيق جدول البيانات مرة أخرى استخدام المعلومات من ملف الاتصال الخارجي بدلاً من كائن الاتصال المضمن في المصنف. |
| [OnlyUseConnectionFile](../../aspose.cells.externalconnections/externalconnection/onlyuseconnectionfile) { get; set; } | يشير إلى ما إذا كان يجب على تطبيق جدول البيانات دائمًا استخدام معلومات الاتصال في ملف الاتصال الخارجي المشار إليه بواسطة السمة odcFile عند تحديث الاتصال. إذا كانت خاطئة ، فيجب أن يتبع تطبيق جدول البيانات الإجراء المشار إليه بواسطة سمة طريقة إعادة الاتصال |
| [Parameters](../../aspose.cells.externalconnections/externalconnection/parameters) { get; } | يحصل[`ConnectionParameterCollection`](../connectionparametercollection) لاستعلام ODBC أو الويب. |
| override [PowerQueryFormula](../../aspose.cells.externalconnections/dbconnection/powerqueryformula) { get; } | يحصل على تعريف صيغة استعلام الطاقة. |
| [ReconnectionMethodType](../../aspose.cells.externalconnections/externalconnection/reconnectionmethodtype) { get; set; } | يحدد ما يجب أن يفعله تطبيق جدول البيانات عند فشل الاتصال . القيمة الافتراضية هي ReConnectionMethodType.Required. |
| [RefreshInternal](../../aspose.cells.externalconnections/externalconnection/refreshinternal) { get; set; } | يحدد عدد الدقائق بين عمليات التحديث التلقائية للاتصال. |
| [RefreshOnLoad](../../aspose.cells.externalconnections/externalconnection/refreshonload) { get; set; } | صحيح إذا كان يجب تحديث هذا الاتصال عند فتح الملف ؛ وإلا ، خطأ . |
| [SaveData](../../aspose.cells.externalconnections/externalconnection/savedata) { get; set; } | صحيح إذا كان سيتم حفظ البيانات الخارجية التي تم جلبها عبر الاتصال لملء جدول مع المصنف ؛ خلاف ذلك ، خطأ. |
| [SavePassword](../../aspose.cells.externalconnections/externalconnection/savepassword) { get; set; } | صحيح إذا كان سيتم حفظ كلمة المرور كجزء من سلسلة الاتصال ؛ وإلا ، خطأ. |
| [SeverCommand](../../aspose.cells.externalconnections/dbconnection/severcommand) { get; set; } | تحديد سلسلة نصية للأمر الثاني تستمر عندما تكون حقول الصفحة المستندة إلى الخادم PivotTable قيد الاستخدام. بالنسبة لاتصالات ODBC ، يكون serverCommand عادةً استعلامًا أوسع من الأمر (لا توجد عبارة WHERE في السابق). استنادًا إلى هذين الأمرين (الأوامر و ServerCommand) ، يمكن ملء واجهة مستخدم المعلمة ويمكن إنشاء الاستعلامات ذات المعلمات |
| [SourceFile](../../aspose.cells.externalconnections/externalconnection/sourcefile) { get; set; } | يُستخدم عندما يكون مصدر البيانات الخارجي مستندًا إلى الملف. عند فشل الاتصال بمصدر بيانات ، يحاول تطبيق جدول البيانات الاتصال مباشرة بهذا الملف. قد يتم التعبير عنه في URI أو بتدوين مسار الملف الخاص بالنظام. |
| [SSOId](../../aspose.cells.externalconnections/externalconnection/ssoid) { get; set; } | معرّف للدخول الأحادي (SSO) يُستخدم للمصادقة بين خادم وسيط spreadsheetML ومصدر البيانات الخارجي. |
| [Type](../../aspose.cells.externalconnections/externalconnection/type) { get; set; } | الحصول على أو تعيين نوع مصدر بيانات الاتصال الخارجي. |

### أنظر أيضا

* class [ExternalConnection](../externalconnection)
* مساحة الاسم [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections)
* المجسم [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
