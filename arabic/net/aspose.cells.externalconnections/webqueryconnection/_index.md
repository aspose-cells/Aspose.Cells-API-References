---
title: WebQueryConnection
second_title: Aspose.Cells لمرجع .NET API
description: تحديد خصائص مصدر استعلام ويب. سيقوم استعلام الويب باسترداد البيانات من جداول HTML  ويمكن أيضًا توفير معلمات HTTP Get ليتم معالجتها بواسطة خادم الويب في إنشاء HTML بواسطة بما في ذلك المعلمات وعناصر المعلمات .
type: docs
weight: 3350
url: /ar/net/aspose.cells.externalconnections/webqueryconnection/
---
## WebQueryConnection class

تحديد خصائص مصدر استعلام ويب. سيقوم استعلام الويب باسترداد البيانات من جداول HTML ، ويمكن أيضًا توفير معلمات HTTP "Get" ليتم معالجتها بواسطة خادم الويب في إنشاء HTML بواسطة بما في ذلك المعلمات وعناصر المعلمات .

```csharp
public class WebQueryConnection : ExternalConnection
```

## الخصائص

| اسم | وصف |
| --- | --- |
| [BackgroundRefresh](../../aspose.cells.externalconnections/externalconnection/backgroundrefresh) { get; set; } | يشير إلى ما إذا كان يمكن تحديث الاتصال في الخلفية (بشكل غير متزامن). true إذا كان الاستخدام المفضل للاتصال هو التحديث غير المتزامن في الخلفية ؛ خطأ إذا كان الاستخدام المفضل للاتصال هو التحديث المتزامن في المقدمة. |
| [ConnectionDescription](../../aspose.cells.externalconnections/externalconnection/connectiondescription) { get; set; } | تحديد وصف المستخدم لهذا الاتصال |
| [ConnectionId](../../aspose.cells.externalconnections/externalconnection/connectionid) { get; } | يحدد المعرف الفريد لهذا الاتصال. |
| [CredentialsMethodType](../../aspose.cells.externalconnections/externalconnection/credentialsmethodtype) { get; set; } | يحدد طريقة المصادقة التي سيتم استخدامها عند إنشاء (أو إعادة تأسيس) الاتصال . |
| [EditWebPage](../../aspose.cells.externalconnections/webqueryconnection/editwebpage) { get; set; } | عنوان URL لصفحة الويب التي تواجه المستخدم والتي تعرض بيانات استعلام الويب. عنوان URL هذا هو persisted في حالة أن sourceData = "true" وتم إعادة توجيه عنوان url للإشارة إلى ملف XML . ثم يمكن إظهار الصفحة التي تواجه المستخدم في واجهة المستخدم ، ويمكن استرداد بيانات XML خلف الكواليس. |
| [HtmlFormat](../../aspose.cells.externalconnections/webqueryconnection/htmlformat) { get; set; } | كيفية معالجة التنسيق من مصدر HTML عند إحضار بيانات استعلام الويب إلى ورقة العمل . تكون ذات صلة عندما تكون بيانات المصدر صحيحة. |
| [Id](../../aspose.cells.externalconnections/externalconnection/id) { get; } | يحصل على معرف الاتصال. |
| [IsConsecutive](../../aspose.cells.externalconnections/webqueryconnection/isconsecutive) { get; set; } | إشارة تشير إلى ما إذا كان يجب معاملة المحددات المتتالية كمحدد واحد فقط. |
| [IsDeleted](../../aspose.cells.externalconnections/externalconnection/isdeleted) { get; set; } | يشير إلى ما إذا كان قد تم حذف اتصال المصنف المرتبط. صحيح إذا تم حذف الاتصال ؛ وإلا ، خطأ . |
| [IsHtmlTables](../../aspose.cells.externalconnections/webqueryconnection/ishtmltables) { get; set; } | علامة تشير إلى ما إذا كانت استعلامات الويب يجب أن تعمل فقط على جداول HTML. |
| [IsNew](../../aspose.cells.externalconnections/externalconnection/isnew) { get; set; } | True إذا لم يتم تحديث الاتصال لأول مرة ؛ خلاف ذلك ، خطأ. يمكن أن تحدث هذه الحالة عندما يحفظ المستخدم الملف قبل انتهاء استعلام العودة. |
| [IsParsePre](../../aspose.cells.externalconnections/webqueryconnection/isparsepre) { get; set; } | علامة تشير إلى ما إذا كانت البيانات الموجودة في علامات HTML PRE في صفحة الويب يتم تحليلها في أعمدة عند استيراد الصفحة إلى جدول استعلام. |
| [IsSameSettings](../../aspose.cells.externalconnections/webqueryconnection/issamesettings) { get; set; } | علامة تشير إلى ما إذا كان سيتم تحليل كافة الجداول داخل كتلة PRE بنفس إعدادات العرض مثل الصف الأول. |
| [IsTextDates](../../aspose.cells.externalconnections/webqueryconnection/istextdates) { get; set; } | علامة تشير إلى ما إذا كان يجب استيراد التواريخ إلى الخلايا في ورقة العمل كنص بدلاً من التواريخ. |
| [IsXl2000](../../aspose.cells.externalconnections/webqueryconnection/isxl2000) { get; set; } | توجد هذه العلامة للتوافق مع الإصدارات السابقة من ملفات جداول البيانات الحالية ، ويتم تعيينها إلى true إذا تم تحديث استعلام الويب هذا في تطبيق جدول بيانات أحدث من Microsoft Excel 2000 أو يساوي هذه سمة اختيارية يمكن تجاهلها . |
| [IsXl97](../../aspose.cells.externalconnections/webqueryconnection/isxl97) { get; set; } | توجد هذه العلامة للتوافق مع الإصدارات السابقة من ملفات جداول البيانات الحالية ، ويتم تعيينها إلى true إذا تم إنشاء استعلام الويب هذا في Microsoft Excel 97. هذه سمة اختيارية يمكن تجاهلها. |
| [IsXml](../../aspose.cells.externalconnections/webqueryconnection/isxml) { get; set; } | صحيح إذا كان مصدر استعلام الويب هو XML (مقابل HTML) ، وإلا يكون خطأ. |
| [IsXmlSourceData](../../aspose.cells.externalconnections/webqueryconnection/isxmlsourcedata) { get; set; } | علامة تشير إلى أنه يجب استيراد بيانات مصدر XML بدلاً من جدول HTML نفسه. |
| [KeepAlive](../../aspose.cells.externalconnections/externalconnection/keepalive) { get; set; } | يكون هذا صحيحًا عندما يجب أن يبذل تطبيق جدول البيانات جهودًا لإبقاء الاتصال مفتوحًا. عندما يكون خطأ ، يجب أن يغلق التطبيق الاتصال بعد استرداد معلومات . |
| [Name](../../aspose.cells.externalconnections/externalconnection/name) { get; set; } | يحدد اسم الاتصال. يجب أن يكون لكل اتصال اسم فريد. |
| [OdcFile](../../aspose.cells.externalconnections/externalconnection/odcfile) { get; set; } | يحدد المسار الكامل لملف الاتصال الخارجي الذي تم إنشاء هذا الاتصال منه. إذا فشل الاتصال أثناء محاولة تحديث البيانات ، وطريقة إعادة الاتصال = 1 ، فسيحاول تطبيق جدول البيانات مرة أخرى استخدام المعلومات من ملف الاتصال الخارجي بدلاً من كائن الاتصال المضمن في المصنف. |
| [OnlyUseConnectionFile](../../aspose.cells.externalconnections/externalconnection/onlyuseconnectionfile) { get; set; } | يشير إلى ما إذا كان يجب على تطبيق جدول البيانات دائمًا استخدام معلومات الاتصال في ملف الاتصال الخارجي المشار إليه بواسطة السمة odcFile عند تحديث الاتصال. إذا كانت خاطئة ، فيجب أن يتبع تطبيق جدول البيانات الإجراء المشار إليه بواسطة سمة طريقة إعادة الاتصال |
| [Parameters](../../aspose.cells.externalconnections/externalconnection/parameters) { get; } | يحصل[`ConnectionParameterCollection`](../connectionparametercollection) لاستعلام ODBC أو الويب. |
| [Post](../../aspose.cells.externalconnections/webqueryconnection/post) { get; set; } | إرجاع أو تعيين السلسلة المستخدمة مع طريقة النشر لإدخال البيانات في خادم ويب لإرجاع البيانات من استعلام ويب. |
| virtual [PowerQueryFormula](../../aspose.cells.externalconnections/externalconnection/powerqueryformula) { get; } | يحصل على تعريف صيغة استعلام الطاقة. |
| [ReconnectionMethodType](../../aspose.cells.externalconnections/externalconnection/reconnectionmethodtype) { get; set; } | يحدد ما يجب أن يفعله تطبيق جدول البيانات عند فشل الاتصال . القيمة الافتراضية هي ReConnectionMethodType.Required. |
| [RefreshInternal](../../aspose.cells.externalconnections/externalconnection/refreshinternal) { get; set; } | يحدد عدد الدقائق بين عمليات التحديث التلقائية للاتصال. |
| [RefreshOnLoad](../../aspose.cells.externalconnections/externalconnection/refreshonload) { get; set; } | صحيح إذا كان يجب تحديث هذا الاتصال عند فتح الملف ؛ وإلا ، خطأ . |
| [SaveData](../../aspose.cells.externalconnections/externalconnection/savedata) { get; set; } | صحيح إذا كان سيتم حفظ البيانات الخارجية التي تم جلبها عبر الاتصال لملء جدول مع المصنف ؛ خلاف ذلك ، خطأ. |
| [SavePassword](../../aspose.cells.externalconnections/externalconnection/savepassword) { get; set; } | صحيح إذا كان سيتم حفظ كلمة المرور كجزء من سلسلة الاتصال ؛ وإلا ، خطأ. |
| [SourceFile](../../aspose.cells.externalconnections/externalconnection/sourcefile) { get; set; } | يُستخدم عندما يكون مصدر البيانات الخارجي مستندًا إلى الملف. عند فشل الاتصال بمصدر بيانات ، يحاول تطبيق جدول البيانات الاتصال مباشرة بهذا الملف. قد يتم التعبير عنه في URI أو بتدوين مسار الملف الخاص بالنظام. |
| [SSOId](../../aspose.cells.externalconnections/externalconnection/ssoid) { get; set; } | معرّف للدخول الأحادي (SSO) يُستخدم للمصادقة بين خادم وسيط spreadsheetML ومصدر البيانات الخارجي. |
| [Type](../../aspose.cells.externalconnections/externalconnection/type) { get; set; } | الحصول على أو تعيين نوع مصدر بيانات الاتصال الخارجي. |
| [Url](../../aspose.cells.externalconnections/webqueryconnection/url) { get; set; } | عنوان URL المراد استخدامه لتحديث البيانات الخارجية . |

### أنظر أيضا

* class [ExternalConnection](../externalconnection)
* مساحة الاسم [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections)
* المجسم [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
