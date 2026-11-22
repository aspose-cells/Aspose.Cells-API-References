---
title: "الفئة WebQueryConnection"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.ExternalConnections.WebQueryConnection. تحدد الخصائص لمصدر استعلام ويب. سيسترجع استعلام الويب البيانات من جداول HTML ويمكنه أيضًا تزويد معلمات HTTP Get لتتم معالجتها بواسطة خادم الويب عند إنشاء HTML عن طريق تضمين المعلمات وعناصر المعلمات"
type: docs
url: /ar/net/aspose.cells.externalconnections/webqueryconnection/
---
## WebQueryConnection class

يحدد الخصائص لمصدر استعلام الويب. سيسترجع استعلام الويب البيانات من جداول HTML، ويمكنه أيضاً تزويد معلمات HTTP "Get" لتتم معالجتها بواسطة خادم الويب عند توليد HTML من خلال تضمين المعلمات وعناصر المعلمات.

```csharp
public class WebQueryConnection : ExternalConnection
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [BackgroundRefresh](../../aspose.cells.externalconnections/externalconnection/backgroundrefresh/) { get; set; } | يشير إلى ما إذا كان يمكن تحديث الاتصال في الخلفية (بشكل غير متزامن). true إذا كان الاستخدام المفضل للاتصال هو التحديث غير المتزامن في الخلفية؛ false إذا كان الاستخدام المفضل هو التحديث المتزامن في الواجهة الأمامية. (موروث من [`ExternalConnection`](../externalconnection/).) |
| override [ClassType](../../aspose.cells.externalconnections/webqueryconnection/classtype/) { get; } | يحصل على نوع كائن [`ExternalConnection`](../externalconnection/) هذا. |
| virtual [Command](../../aspose.cells.externalconnections/externalconnection/command/) { get; set; } | السلسلة التي تحتوي على أمر قاعدة البيانات لتمريره إلى واجهة برمجة تطبيقات موفر البيانات التي ستتفاعل مع المصدر الخارجي لاسترجاع البيانات (موروثة من [`ExternalConnection`](../externalconnection/).) |
| virtual [CommandType](../../aspose.cells.externalconnections/externalconnection/commandtype/) { get; set; } | يحدد نوع أمر OLE DB. 1. الاستعلام يحدد اسم المكعب 2. الاستعلام يحدد عبارة SQL 3. الاستعلام يحدد اسم الجدول 4. الاستعلام يحدد أنه تم تقديم المعلومات الافتراضية، ويعتمد على الموفر كيفية تفسيرها. 5. الاستعلام ضد موفر بيانات قائمة قائم على الويب. (موروثة من [`ExternalConnection`](../externalconnection/).) |
| [ConnectionDescription](../../aspose.cells.externalconnections/externalconnection/connectiondescription/) { get; set; } | يحدد الوصف الذي يدخله المستخدم لهذا الاتصال (موروث من [`ExternalConnection`](../externalconnection/).) |
| override [ConnectionFile](../../aspose.cells.externalconnections/webqueryconnection/connectionfile/) { get; } | يحصل على ملف الاتصال. |
| [ConnectionId](../../aspose.cells.externalconnections/externalconnection/connectionid/) { get; } | (**Obsolete.**) يحدد المعرف الفريد لهذا الاتصال. (موروث من [`ExternalConnection`](../externalconnection/).) |
| virtual [ConnectionString](../../aspose.cells.externalconnections/externalconnection/connectionstring/) { get; set; } | يُستخدم سلسلة معلومات الاتصال لإجراء اتصال بمصدر بيانات OLE DB أو ODBC. (موروثة من [`ExternalConnection`](../externalconnection/).) |
| [Credentials](../../aspose.cells.externalconnections/externalconnection/credentials/) { get; set; } | (**Obsolete.**) يحدد طريقة المصادقة التي تُستخدم عند إنشاء (أو إعادة إنشاء) الاتصال. (موروث من [`ExternalConnection`](../externalconnection/).) |
| [CredentialsMethodType](../../aspose.cells.externalconnections/externalconnection/credentialsmethodtype/) { get; set; } | يحدد طريقة المصادقة التي تُستخدم عند إنشاء (أو إعادة إنشاء) الاتصال. (موروث من [`ExternalConnection`](../externalconnection/).) |
| [EditPage](../../aspose.cells.externalconnections/webqueryconnection/editpage/) { get; set; } | (**مهمل.**) عنوان URL للصفحة الويب الموجهة للمستخدم والتي تعرض بيانات استعلام الويب. يتم حفظ هذا العنوان في الحالة التي تكون فيها sourceData="true" وتم إعادة توجيه url للإشارة إلى ملف XML. ثم يمكن عرض الصفحة الموجهة للمستخدم في واجهة المستخدم، ويمكن استرجاع بيانات XML خلف الكواليس. |
| [EditWebPage](../../aspose.cells.externalconnections/webqueryconnection/editwebpage/) { get; set; } | عنوان URL للصفحة الويب الموجهة للمستخدم والتي تعرض بيانات استعلام الويب. يتم حفظ هذا العنوان في الحالة التي تكون فيها sourceData="true" وتم إعادة توجيه url للإشارة إلى ملف XML. ثم يمكن عرض الصفحة الموجهة للمستخدم في واجهة المستخدم، ويمكن استرجاع بيانات XML خلف الكواليس. |
| [HtmlFormat](../../aspose.cells.externalconnections/webqueryconnection/htmlformat/) { get; set; } | كيفية معالجة التنسيق من مصدر HTML عند جلب بيانات استعلام الويب إلى ورقة العمل. ذو صلة عندما تكون sourceData صحيحة. |
| [Id](../../aspose.cells.externalconnections/externalconnection/id/) { get; } | يحصل على معرف الاتصال. (موروث من [`ExternalConnection`](../externalconnection/).) |
| [IsConsecutive](../../aspose.cells.externalconnections/webqueryconnection/isconsecutive/) { get; set; } | علامة تشير إلى ما إذا كان يجب معالجة الفواصل المتتالية كفاصل واحد فقط. |
| [IsDeleted](../../aspose.cells.externalconnections/externalconnection/isdeleted/) { get; set; } | يشير إلى ما إذا كان اتصال المصنف المرتبط قد تم حذفه. true إذا تم حذف الاتصال؛ وإلا false. (موروث من [`ExternalConnection`](../externalconnection/).) |
| [IsHtmlTables](../../aspose.cells.externalconnections/webqueryconnection/ishtmltables/) { get; set; } | علامة تشير إلى ما إذا كان يجب أن تعمل استعلامات الويب فقط على جداول HTML. |
| [IsNew](../../aspose.cells.externalconnections/externalconnection/isnew/) { get; set; } | true إذا لم يتم تحديث الاتصال للمرة الأولى؛ وإلا false. يمكن أن يحدث هذا الوضع عندما يحفظ المستخدم الملف قبل إكمال الاستعلام. (موروث من [`ExternalConnection`](../externalconnection/).) |
| [IsParsePre](../../aspose.cells.externalconnections/webqueryconnection/isparsepre/) { get; set; } | علامة تشير إلى ما إذا كانت البيانات الموجودة داخل وسوم HTML PRE في صفحة الويب تُحلل إلى أعمدة عند استيراد الصفحة إلى جدول استعلام. |
| [IsSameSettings](../../aspose.cells.externalconnections/webqueryconnection/issamesettings/) { get; set; } | علامة تشير إلى ما إذا كان يجب تحليل جميع الجداول داخل كتلة PRE بنفس إعدادات العرض للصف الأول. |
| [IsTextDates](../../aspose.cells.externalconnections/webqueryconnection/istextdates/) { get; set; } | علامة تشير إلى ما إذا كان يجب استيراد التواريخ إلى خلايا ورقة العمل كنص بدلاً من تواريخ. |
| [IsXl2000](../../aspose.cells.externalconnections/webqueryconnection/isxl2000/) { get; set; } | هذه العلامة موجودة لتوافقية مع ملفات الجداول الإلكترونية القديمة الموجودة، وتُضبط على true إذا تم تحديث هذا الاستعلام الويب في تطبيق جدول إلكتروني أحدث من أو يساوي Microsoft Excel 2000. هذه خاصية اختيارية يمكن تجاهلها. |
| [IsXl97](../../aspose.cells.externalconnections/webqueryconnection/isxl97/) { get; set; } | هذه العلامة موجودة لتوافقية مع ملفات الجداول الإلكترونية القديمة الموجودة، وتُضبط على true إذا تم إنشاء هذا الاستعلام الويب في Microsoft Excel 97. هذه خاصية اختيارية يمكن تجاهلها. |
| [IsXml](../../aspose.cells.externalconnections/webqueryconnection/isxml/) { get; set; } | true إذا كان مصدر الاستعلام الويب هو XML (مقابل HTML)، وإلا false. |
| [IsXmlSourceData](../../aspose.cells.externalconnections/webqueryconnection/isxmlsourcedata/) { get; set; } | علامة تشير إلى أنه يجب استيراد بيانات المصدر XML بدلاً من جدول HTML نفسه. |
| [KeepAlive](../../aspose.cells.externalconnections/externalconnection/keepalive/) { get; set; } | true عندما يجب على تطبيق الجداول الإلكترونية السعي لإبقاء الاتصال مفتوحًا. عندما يكون false، يجب على التطبيق إغلاق الاتصال بعد استرجاع المعلومات. (موروث من [`ExternalConnection`](../externalconnection/).) |
| [Name](../../aspose.cells.externalconnections/externalconnection/name/) { get; set; } | يحدد اسم الاتصال. يجب أن يكون لكل اتصال اسم فريد. (موروث من [`ExternalConnection`](../externalconnection/).) |
| [OdcFile](../../aspose.cells.externalconnections/externalconnection/odcfile/) { get; set; } | يحدد المسار الكامل لملف الاتصال الخارجي الذي تم إنشاء هذا الاتصال منه. إذا فشل الاتصال أثناء محاولة تحديث البيانات، وكان reconnectionMethod=1، فستحاول تطبيق الجداول الإلكترونية مرة أخرى باستخدام المعلومات من ملف الاتصال الخارجي بدلاً من كائن الاتصال المدمج داخل المصنف.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [OnlyUseConnectionFile](../../aspose.cells.externalconnections/externalconnection/onlyuseconnectionfile/) { get; set; } | يحدد ما إذا كان يجب على تطبيق الجداول الإلكترونية دائمًا وفقط استخدام معلومات الاتصال الموجودة في ملف الاتصال الخارجي المشار إليه بصفة odcFile عند تحديث الاتصال. إذا كان false، يجب على تطبيق الجداول الإلكترونية اتباع الإجراء المشار إليه بصفة reconnectionMethod(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [Parameters](../../aspose.cells.externalconnections/externalconnection/parameters/) { get; } | يحصل على [`ConnectionParameterCollection`](../connectionparametercollection/) لاستعلام ODBC أو ويب.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [Post](../../aspose.cells.externalconnections/webqueryconnection/post/) { get; set; } | تُرجع أو تُعيّن السلسلة المستخدمة مع طريقة post لإدخال البيانات إلى خادم ويب لإرجاع البيانات من استعلام ويب. |
| virtual [PowerQueryFormula](../../aspose.cells.externalconnections/externalconnection/powerqueryformula/) { get; } | يحصل على تعريف صيغة Power Query.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [ReconnectionMethod](../../aspose.cells.externalconnections/externalconnection/reconnectionmethod/) { get; set; } | (**Obsolete.**) يحدد ما يجب على تطبيق الجداول الإلكترونية القيام به عندما يفشل الاتصال. القيمة الافتراضية هي ReConnectionMethodType.Required.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [ReconnectionMethodType](../../aspose.cells.externalconnections/externalconnection/reconnectionmethodtype/) { get; set; } | يحدد ما يجب على تطبيق الجداول الإلكترونية القيام به عندما يفشل الاتصال. القيمة الافتراضية هي ReConnectionMethodType.Required.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [RefreshInternal](../../aspose.cells.externalconnections/externalconnection/refreshinternal/) { get; set; } | يحدد عدد الدقائق بين عمليات التحديث التلقائي للاتصال.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [RefreshOnLoad](../../aspose.cells.externalconnections/externalconnection/refreshonload/) { get; set; } | True إذا كان يجب تحديث هذا الاتصال عند فتح الملف؛ وإلا false.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [SaveData](../../aspose.cells.externalconnections/externalconnection/savedata/) { get; set; } | True إذا كان يجب حفظ البيانات الخارجية التي تم جلبها عبر الاتصال لتعبئة جدول مع المصنف؛ وإلا false.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [SavePassword](../../aspose.cells.externalconnections/externalconnection/savepassword/) { get; set; } | True إذا كان يجب حفظ كلمة المرور كجزء من سلسلة الاتصال؛ وإلا False.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| virtual [SecondCommand](../../aspose.cells.externalconnections/externalconnection/secondcommand/) { get; set; } | يحدد سلسلة نص الأمر الثانية التي تُحفظ عندما تكون حقول الصفحة المستندة إلى الخادم في PivotTable قيد الاستخدام. بالنسبة لاتصالات ODBC، يكون serverCommand عادةً استعلامًا أوسع من command (لا توجد جملة WHERE في الأول). استنادًا إلى هذين الأمرين (Command و ServerCommand)، يمكن ملء واجهة المستخدم للمعلمات ويمكن إنشاء استعلامات معلمة (موروثة من [`ExternalConnection`](../externalconnection/).) |
| [SourceFile](../../aspose.cells.externalconnections/externalconnection/sourcefile/) { get; set; } | يُستخدم عندما يكون مصدر البيانات الخارجي قائمًا على ملف. عندما يفشل الاتصال بمثل هذا المصدر، يحاول تطبيق الجداول الإلكترونية الاتصال مباشرةً بهذا الملف. قد يُعبّر عنه في URI أو بصيغة مسار ملف خاص بالنظام.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [SourceType](../../aspose.cells.externalconnections/externalconnection/sourcetype/) { get; set; } | يحصل على أو يحدد نوع DataSource للاتصال الخارجي.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [SSOId](../../aspose.cells.externalconnections/externalconnection/ssoid/) { get; set; } | معرف الدخول الأحادي (SSO) المستخدم للمصادقة بين خادم spreadsheetML وسيط ومصدر البيانات الخارجي.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [Type](../../aspose.cells.externalconnections/externalconnection/type/) { get; set; } | (**Obsolete.**) يحصل على أو يحدد نوع DataSource للاتصال الخارجي.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [Url](../../aspose.cells.externalconnections/webqueryconnection/url/) { get; set; } | URL لاستخدامه لتحديث البيانات الخارجية. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionsClassWebQueryConnectionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();

            try
            {
                // إنشاء اتصال استعلام ويب عبر المجموعة
                WebQueryConnection connection = (WebQueryConnection)workbook.DataConnections[workbook.DataConnections.Count];
                
                connection.Url = "https://example.com/financial-data";
                connection.IsHtmlTables = true;
                connection.IsTextDates = true;
                connection.HtmlFormat = HtmlFormatHandlingType.All;

                Console.WriteLine($"Web query URL: {connection.Url}");
                Console.WriteLine($"HTML tables only: {connection.IsHtmlTables}");

                workbook.Save("WebQueryConnectionDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with WebQueryConnection: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [ExternalConnection](../externalconnection/)
* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


