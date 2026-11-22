---
title: "الفئة DataModelConnection"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.ExternalConnections.DataModelConnection. يحدد اتصال نموذج بيانات"
type: docs
url: /ar/net/aspose.cells.externalconnections/datamodelconnection/
---
## DataModelConnection class

يحدد اتصال نموذج البيانات

```csharp
public class DataModelConnection : ExternalConnection
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [BackgroundRefresh](../../aspose.cells.externalconnections/externalconnection/backgroundrefresh/) { get; set; } | يشير إلى ما إذا كان يمكن تحديث الاتصال في الخلفية (بشكل غير متزامن). true إذا كان الاستخدام المفضل للاتصال هو التحديث غير المتزامن في الخلفية؛ false إذا كان الاستخدام المفضل هو التحديث المتزامن في الواجهة الأمامية. (موروث من [`ExternalConnection`](../externalconnection/).) |
| override [ClassType](../../aspose.cells.externalconnections/datamodelconnection/classtype/) { get; } | يحصل على نوع كائن [`ExternalConnection`](../externalconnection/) هذا. |
| override [Command](../../aspose.cells.externalconnections/datamodelconnection/command/) { get; set; } | السلسلة التي تحتوي على أمر قاعدة البيانات لتمريره إلى واجهة برمجة تطبيقات مزود البيانات التي ستتفاعل مع المصدر الخارجي لاسترجاع البيانات. |
| override [CommandType](../../aspose.cells.externalconnections/datamodelconnection/commandtype/) { get; set; } | يعيد نوع [`OLEDBCommandType`](../oledbcommandtype/). |
| [ConnectionDescription](../../aspose.cells.externalconnections/externalconnection/connectiondescription/) { get; set; } | يحدد الوصف الذي يدخله المستخدم لهذا الاتصال (موروث من [`ExternalConnection`](../externalconnection/).) |
| virtual [ConnectionFile](../../aspose.cells.externalconnections/externalconnection/connectionfile/) { get; } | يحصل على ملف الاتصال. (موروث من [`ExternalConnection`](../externalconnection/).) |
| [ConnectionId](../../aspose.cells.externalconnections/externalconnection/connectionid/) { get; } | (**Obsolete.**) يحدد المعرف الفريد لهذا الاتصال. (موروث من [`ExternalConnection`](../externalconnection/).) |
| override [ConnectionString](../../aspose.cells.externalconnections/datamodelconnection/connectionstring/) { get; set; } | سلسلة معلومات الاتصال تُستخدم لإجراء اتصال بمصدر بيانات OLE DB أو ODBC. |
| [Credentials](../../aspose.cells.externalconnections/externalconnection/credentials/) { get; set; } | (**Obsolete.**) يحدد طريقة المصادقة التي تُستخدم عند إنشاء (أو إعادة إنشاء) الاتصال. (موروث من [`ExternalConnection`](../externalconnection/).) |
| [CredentialsMethodType](../../aspose.cells.externalconnections/externalconnection/credentialsmethodtype/) { get; set; } | يحدد طريقة المصادقة التي تُستخدم عند إنشاء (أو إعادة إنشاء) الاتصال. (موروث من [`ExternalConnection`](../externalconnection/).) |
| [Id](../../aspose.cells.externalconnections/externalconnection/id/) { get; } | يحصل على معرف الاتصال. (موروث من [`ExternalConnection`](../externalconnection/).) |
| [IsDeleted](../../aspose.cells.externalconnections/externalconnection/isdeleted/) { get; set; } | يشير إلى ما إذا كان اتصال المصنف المرتبط قد تم حذفه. true إذا تم حذف الاتصال؛ وإلا false. (موروث من [`ExternalConnection`](../externalconnection/).) |
| [IsNew](../../aspose.cells.externalconnections/externalconnection/isnew/) { get; set; } | true إذا لم يتم تحديث الاتصال للمرة الأولى؛ وإلا false. يمكن أن يحدث هذا الوضع عندما يحفظ المستخدم الملف قبل إكمال الاستعلام. (موروث من [`ExternalConnection`](../externalconnection/).) |
| [KeepAlive](../../aspose.cells.externalconnections/externalconnection/keepalive/) { get; set; } | true عندما يجب على تطبيق الجداول الإلكترونية السعي لإبقاء الاتصال مفتوحًا. عندما يكون false، يجب على التطبيق إغلاق الاتصال بعد استرجاع المعلومات. (موروث من [`ExternalConnection`](../externalconnection/).) |
| [Name](../../aspose.cells.externalconnections/externalconnection/name/) { get; set; } | يحدد اسم الاتصال. يجب أن يكون لكل اتصال اسم فريد. (موروث من [`ExternalConnection`](../externalconnection/).) |
| [OdcFile](../../aspose.cells.externalconnections/externalconnection/odcfile/) { get; set; } | يحدد المسار الكامل لملف الاتصال الخارجي الذي تم إنشاء هذا الاتصال منه. إذا فشل الاتصال أثناء محاولة تحديث البيانات، وكان reconnectionMethod=1، فستحاول تطبيق الجداول الإلكترونية مرة أخرى باستخدام المعلومات من ملف الاتصال الخارجي بدلاً من كائن الاتصال المدمج داخل المصنف.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [OnlyUseConnectionFile](../../aspose.cells.externalconnections/externalconnection/onlyuseconnectionfile/) { get; set; } | يحدد ما إذا كان يجب على تطبيق الجداول الإلكترونية دائمًا وفقط استخدام معلومات الاتصال الموجودة في ملف الاتصال الخارجي المشار إليه بصفة odcFile عند تحديث الاتصال. إذا كان false، يجب على تطبيق الجداول الإلكترونية اتباع الإجراء المشار إليه بصفة reconnectionMethod(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [Parameters](../../aspose.cells.externalconnections/externalconnection/parameters/) { get; } | يحصل على [`ConnectionParameterCollection`](../connectionparametercollection/) لاستعلام ODBC أو ويب.(Inherited from [`ExternalConnection`](../externalconnection/).) |
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

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;
    using System.Collections.Generic;

    public class ExternalConnectionsClassDataModelConnectionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد للعرض
            Workbook workbook = new Workbook();

            try
            {
                // إنشاء نسخة من فئة DataModelConnection باستخدام الانعكاس
                DataModelConnection connection = (DataModelConnection)System.Runtime.Serialization.FormatterServices.GetUninitializedObject(typeof(DataModelConnection));

                // ضبط الخصائص الأساسية
                connection.Command = "SELECT * FROM Products";
                connection.CommandType = OLEDBCommandType.SqlStatement;
                connection.ConnectionString = "Provider=SQLOLEDB;Data Source=Northwind;Integrated Security=SSPI";

                // إضافة الاتصال إلى اتصالات البيانات في المصنف
                ((IList<ExternalConnection>)workbook.DataConnections).Add(connection);

                // عرض معلومات الاتصال
                Console.WriteLine($"Connection Type: {connection.ClassType}");
                Console.WriteLine($"Command: {connection.Command}");
                Console.WriteLine($"Command Type: {connection.CommandType}");
                Console.WriteLine($"Connection String: {connection.ConnectionString}");

                // احفظ المصنف
                workbook.Save("DataModelConnectionDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with DataModelConnection.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with DataModelConnection: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [ExternalConnection](../externalconnection/)
* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


