---
title: "الفئة DBConnection."
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.ExternalConnections.DBConnection. تحدد جميع الخصائص المرتبطة باتصال بيانات خارجي ODBC أو OLE DB."
type: docs
url: /ar/net/aspose.cells.externalconnections/dbconnection/
---
## DBConnection class

يحدد جميع الخصائص المرتبطة باتصال بيانات خارجي ODBC أو OLE DB.

```csharp
public class DBConnection : ExternalConnection
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [BackgroundRefresh](../../aspose.cells.externalconnections/externalconnection/backgroundrefresh/) { get; set; } | يشير إلى ما إذا كان يمكن تحديث الاتصال في الخلفية (بشكل غير متزامن). true إذا كان الاستخدام المفضل للاتصال هو التحديث غير المتزامن في الخلفية؛ false إذا كان الاستخدام المفضل هو التحديث المتزامن في الواجهة الأمامية. (موروث من [`ExternalConnection`](../externalconnection/).) |
| override [ClassType](../../aspose.cells.externalconnections/dbconnection/classtype/) { get; } | يحصل على نوع كائن [`ExternalConnection`](../externalconnection/) هذا. |
| override [Command](../../aspose.cells.externalconnections/dbconnection/command/) { get; set; } | السلسلة التي تحتوي على أمر قاعدة البيانات لتمريره إلى واجهة برمجة تطبيقات مزود البيانات التي ستتفاعل مع المصدر الخارجي لاسترجاع البيانات. |
| override [CommandType](../../aspose.cells.externalconnections/dbconnection/commandtype/) { get; set; } | يحدد نوع أمر OLE DB. 1. يحدد الاستعلام اسم مكعب 2. يحدد الاستعلام بيان SQL 3. يحدد الاستعلام اسم جدول 4. يحدد الاستعلام أن المعلومات الافتراضية قد تم تقديمها، ويعتمد على المزود كيفية تفسيرها. 5. الاستعلام ضد موفر بيانات قائمة ويب. |
| [ConnectionDescription](../../aspose.cells.externalconnections/externalconnection/connectiondescription/) { get; set; } | يحدد الوصف الذي يدخله المستخدم لهذا الاتصال (موروث من [`ExternalConnection`](../externalconnection/).) |
| virtual [ConnectionFile](../../aspose.cells.externalconnections/externalconnection/connectionfile/) { get; } | يحصل على ملف الاتصال. (موروث من [`ExternalConnection`](../externalconnection/).) |
| [ConnectionId](../../aspose.cells.externalconnections/externalconnection/connectionid/) { get; } | (**Obsolete.**) يحدد المعرف الفريد لهذا الاتصال. (موروث من [`ExternalConnection`](../externalconnection/).) |
| [ConnectionInfo](../../aspose.cells.externalconnections/dbconnection/connectioninfo/) { get; set; } | (**Obsolete.**) تُستخدم سلسلة معلومات الاتصال لإجراء اتصال بمصدر بيانات OLE DB أو ODBC. |
| override [ConnectionString](../../aspose.cells.externalconnections/dbconnection/connectionstring/) { get; set; } | سلسلة معلومات الاتصال تُستخدم لإجراء اتصال بمصدر بيانات OLE DB أو ODBC. |
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
| override [PowerQueryFormula](../../aspose.cells.externalconnections/dbconnection/powerqueryformula/) { get; } | يحصل على تعريف صيغة Power Query. |
| [ReconnectionMethod](../../aspose.cells.externalconnections/externalconnection/reconnectionmethod/) { get; set; } | (**Obsolete.**) يحدد ما يجب على تطبيق الجداول الإلكترونية القيام به عندما يفشل الاتصال. القيمة الافتراضية هي ReConnectionMethodType.Required.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [ReconnectionMethodType](../../aspose.cells.externalconnections/externalconnection/reconnectionmethodtype/) { get; set; } | يحدد ما يجب على تطبيق الجداول الإلكترونية القيام به عندما يفشل الاتصال. القيمة الافتراضية هي ReConnectionMethodType.Required.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [RefreshInternal](../../aspose.cells.externalconnections/externalconnection/refreshinternal/) { get; set; } | يحدد عدد الدقائق بين عمليات التحديث التلقائي للاتصال.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [RefreshOnLoad](../../aspose.cells.externalconnections/externalconnection/refreshonload/) { get; set; } | True إذا كان يجب تحديث هذا الاتصال عند فتح الملف؛ وإلا false.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [SaveData](../../aspose.cells.externalconnections/externalconnection/savedata/) { get; set; } | True إذا كان يجب حفظ البيانات الخارجية التي تم جلبها عبر الاتصال لتعبئة جدول مع المصنف؛ وإلا false.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [SavePassword](../../aspose.cells.externalconnections/externalconnection/savepassword/) { get; set; } | True إذا كان يجب حفظ كلمة المرور كجزء من سلسلة الاتصال؛ وإلا False.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| override [SecondCommand](../../aspose.cells.externalconnections/dbconnection/secondcommand/) { get; set; } | يحدد نص أمر ثانٍ يتم حفظه عندما تكون حقول الصفحات المستندة إلى الخادم في PivotTable قيد الاستخدام. في اتصالات ODBC، عادةً ما يكون serverCommand استعلامًا أوسع من command (لا توجد جملة WHERE في الأول). استنادًا إلى هذين الأمرين (Command و ServerCommand)، يمكن ملء واجهة المستخدم للمعلمات وإنشاء استعلامات معلمة |
| [SeverCommand](../../aspose.cells.externalconnections/dbconnection/severcommand/) { get; set; } | (**Obsolete.**) يحدد نص أمر ثانٍ يتم حفظه عندما تكون حقول الصفحات المستندة إلى الخادم في PivotTable قيد الاستخدام. في اتصالات ODBC، عادةً ما يكون serverCommand استعلامًا أوسع من command (لا توجد جملة WHERE في الأول). استنادًا إلى هذين الأمرين (Command و ServerCommand)، يمكن ملء واجهة المستخدم للمعلمات وإنشاء استعلامات معلمة |
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

    public class ExternalConnectionsClassDBConnectionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد للعرض
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // إنشاء كائن DBConnection جديد بإضافته إلى المجموعة
                var connections = workbook.DataConnections;
                DBConnection dbConnection = (DBConnection)connections[connections.Count];

                // تعيين الخصائص الأساسية
                dbConnection.ConnectionString = "Provider=Microsoft.Jet.OLEDB.4.0;Data Source=C:\\data\\database.mdb;";
                dbConnection.CommandType = OLEDBCommandType.TableName;
                dbConnection.Command = "Customers";

                // عرض الخصائص للقراءة فقط
                Console.WriteLine("DBConnection ClassType: " + dbConnection.ClassType);
                Console.WriteLine("ConnectionString: " + dbConnection.ConnectionString);
                Console.WriteLine("CommandType: " + dbConnection.CommandType);
                Console.WriteLine("Command: " + dbConnection.Command);

                // احفظ المصنف
                workbook.Save("DBConnectionDemo.xlsx");
                Console.WriteLine("DBConnection demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with DBConnection: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [ExternalConnection](../externalconnection/)
* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


