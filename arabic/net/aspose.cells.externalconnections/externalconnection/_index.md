---
title: "الفئة ExternalConnection"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.ExternalConnections.ExternalConnection class. يحدد اتصال بيانات خارجي"
type: docs
url: /ar/net/aspose.cells.externalconnections/externalconnection/
---
## ExternalConnection class

يحدد اتصال بيانات خارجي

```csharp
public abstract class ExternalConnection
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [BackgroundRefresh](../../aspose.cells.externalconnections/externalconnection/backgroundrefresh/) { get; set; } | يشير إلى ما إذا كان يمكن تحديث الاتصال في الخلفية (بشكل غير متزامن). true إذا كان الاستخدام المفضل للاتصال هو التحديث غير المتزامن في الخلفية؛ false إذا كان الاستخدام المفضل للاتصال هو التحديث المتزامن في الواجهة الأمامية. |
| abstract [ClassType](../../aspose.cells.externalconnections/externalconnection/classtype/) { get; } | يحصل على نوع هذا الكائن `ExternalConnection`. |
| virtual [Command](../../aspose.cells.externalconnections/externalconnection/command/) { get; set; } | السلسلة التي تحتوي على أمر قاعدة البيانات لتمريره إلى واجهة برمجة تطبيقات مزود البيانات التي ستتفاعل مع المصدر الخارجي لاسترجاع البيانات. |
| virtual [CommandType](../../aspose.cells.externalconnections/externalconnection/commandtype/) { get; set; } | يحدد نوع أمر OLE DB. 1. يحدد الاستعلام اسم مكعب 2. يحدد الاستعلام بيان SQL 3. يحدد الاستعلام اسم جدول 4. يحدد الاستعلام أن المعلومات الافتراضية قد تم تقديمها، ويعتمد على المزود كيفية تفسيرها. 5. الاستعلام ضد موفر بيانات قائمة ويب. |
| [ConnectionDescription](../../aspose.cells.externalconnections/externalconnection/connectiondescription/) { get; set; } | يحدد الوصف الذي يدخله المستخدم لهذا الاتصال |
| virtual [ConnectionFile](../../aspose.cells.externalconnections/externalconnection/connectionfile/) { get; } | يحصل على ملف الاتصال. |
| [ConnectionId](../../aspose.cells.externalconnections/externalconnection/connectionid/) { get; } | (**Obsolete.**) يحدد المعرف الفريد لهذا الاتصال. |
| virtual [ConnectionString](../../aspose.cells.externalconnections/externalconnection/connectionstring/) { get; set; } | سلسلة معلومات الاتصال تُستخدم لإجراء اتصال بمصدر بيانات OLE DB أو ODBC. |
| [Credentials](../../aspose.cells.externalconnections/externalconnection/credentials/) { get; set; } | (**Obsolete.**) يحدد طريقة المصادقة التي يجب استخدامها عند إنشاء (أو إعادة إنشاء) الاتصال. |
| [CredentialsMethodType](../../aspose.cells.externalconnections/externalconnection/credentialsmethodtype/) { get; set; } | يحدد طريقة المصادقة التي يجب استخدامها عند إنشاء (أو إعادة إنشاء) الاتصال. |
| [Id](../../aspose.cells.externalconnections/externalconnection/id/) { get; } | يحصل على معرف الاتصال. |
| [IsDeleted](../../aspose.cells.externalconnections/externalconnection/isdeleted/) { get; set; } | يشير إلى ما إذا تم حذف اتصال دفتر العمل المرتبط. true إذا تم حذف الاتصال؛ وإلا false. |
| [IsNew](../../aspose.cells.externalconnections/externalconnection/isnew/) { get; set; } | true إذا لم يتم تحديث الاتصال للمرة الأولى؛ وإلا false. يمكن أن يحدث هذا الحالة عندما يقوم المستخدم بحفظ الملف قبل أن ينتهي الاستعلام من الإرجاع. |
| [KeepAlive](../../aspose.cells.externalconnections/externalconnection/keepalive/) { get; set; } | true عندما يجب على تطبيق الجدول الإلكتروني بذل الجهود للحفاظ على الاتصال مفتوحًا. عندما يكون false، يجب على التطبيق إغلاق الاتصال بعد استرجاع المعلومات. |
| [Name](../../aspose.cells.externalconnections/externalconnection/name/) { get; set; } | يحدد اسم الاتصال. يجب أن يكون لكل اتصال اسم فريد. |
| [OdcFile](../../aspose.cells.externalconnections/externalconnection/odcfile/) { get; set; } | يحدد المسار الكامل إلى ملف الاتصال الخارجي الذي تم إنشاء هذا الاتصال منه. إذا فشل الاتصال أثناء محاولة تحديث البيانات، وكان reconnectionMethod=1، فستحاول تطبيق الجدول الإلكتروني مرة أخرى باستخدام المعلومات من ملف الاتصال الخارجي بدلاً من كائن الاتصال المضمن داخل دفتر العمل. |
| [OnlyUseConnectionFile](../../aspose.cells.externalconnections/externalconnection/onlyuseconnectionfile/) { get; set; } | يشير إلى ما إذا كان يجب على تطبيق الجدول الإلكتروني دائمًا واستخدام فقط معلومات الاتصال الموجودة في ملف الاتصال الخارجي المشار إليه بخصية odcFile عند تحديث الاتصال. إذا كان false، يجب على تطبيق الجدول الإلكتروني اتباع الإجراء المشار إليه بخصية reconnectionMethod. |
| [Parameters](../../aspose.cells.externalconnections/externalconnection/parameters/) { get; } | يحصل على [`ConnectionParameterCollection`](../connectionparametercollection/) لاستعلام ODBC أو ويب. |
| virtual [PowerQueryFormula](../../aspose.cells.externalconnections/externalconnection/powerqueryformula/) { get; } | يحصل على تعريف صيغة Power Query. |
| [ReconnectionMethod](../../aspose.cells.externalconnections/externalconnection/reconnectionmethod/) { get; set; } | (**Obsolete.**) يحدد ما يجب على تطبيق الجدول الإلكتروني القيام به عندما يفشل الاتصال. القيمة الافتراضية هي ReConnectionMethodType.Required. |
| [ReconnectionMethodType](../../aspose.cells.externalconnections/externalconnection/reconnectionmethodtype/) { get; set; } | يحدد ما يجب على تطبيق الجدول الإلكتروني القيام به عندما يفشل الاتصال. القيمة الافتراضية هي ReConnectionMethodType.Required. |
| [RefreshInternal](../../aspose.cells.externalconnections/externalconnection/refreshinternal/) { get; set; } | يحدد عدد الدقائق بين عمليات التحديث التلقائي للاتصال. |
| [RefreshOnLoad](../../aspose.cells.externalconnections/externalconnection/refreshonload/) { get; set; } | صحيح إذا كان يجب تحديث هذا الاتصال عند فتح الملف؛ وإلا، خطأ. |
| [SaveData](../../aspose.cells.externalconnections/externalconnection/savedata/) { get; set; } | صحيح إذا كان يجب حفظ البيانات الخارجية التي تم جلبها عبر الاتصال لتعبئة جدول مع المصنف؛ وإلا، خطأ. |
| [SavePassword](../../aspose.cells.externalconnections/externalconnection/savepassword/) { get; set; } | صحيح إذا كان يجب حفظ كلمة المرور كجزء من سلسلة الاتصال؛ وإلا، خطأ. |
| virtual [SecondCommand](../../aspose.cells.externalconnections/externalconnection/secondcommand/) { get; set; } | يحدد نص أمر ثانٍ يتم حفظه عندما تكون حقول الصفحات المستندة إلى الخادم في PivotTable قيد الاستخدام. في اتصالات ODBC، عادةً ما يكون serverCommand استعلامًا أوسع من command (لا توجد جملة WHERE في الأول). استنادًا إلى هذين الأمرين (Command و ServerCommand)، يمكن ملء واجهة المستخدم للمعلمات وإنشاء استعلامات معلمة |
| [SourceFile](../../aspose.cells.externalconnections/externalconnection/sourcefile/) { get; set; } | يُستخدم عندما يكون مصدر البيانات الخارجي معتمدًا على ملف. عندما يفشل الاتصال بمثل هذا المصدر، تحاول تطبيق الجداول الإلكترونية الاتصال مباشرةً بهذا الملف. قد يُعبَّر عنه بصيغة URI أو بصيغة مسار ملف خاص بالنظام. |
| [SourceType](../../aspose.cells.externalconnections/externalconnection/sourcetype/) { get; set; } | يحصل أو يعيّن نوع DataSource للاتصال الخارجي. |
| [SSOId](../../aspose.cells.externalconnections/externalconnection/ssoid/) { get; set; } | معرّف لتقنية الدخول الموحد (Single Sign On (SSO)) المستخدمة للمصادقة بين خادم spreadsheetML وسيط ومصدر البيانات الخارجي. |
| [Type](../../aspose.cells.externalconnections/externalconnection/type/) { get; set; } | (**Obsolete.**) يحصل أو يعيّن نوع DataSource للاتصال الخارجي. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class ExternalConnectionsClassExternalConnectionDemo
    {
        public static void Run()
        {
            string sourceDir = "Your Source Directory";

            Workbook workbook = new Workbook(sourceDir + "example.xlsx");
            ExternalConnectionCollection conns = workbook.DataConnections;
            foreach (ExternalConnection conn in conns)
            {
                if (conn is DBConnection dbConn)
                {
                    Console.WriteLine("Connection Info: " + dbConn.ConnectionInfo);
                    Console.WriteLine("Formula Definition: " + dbConn.PowerQueryFormula.FormulaDefinition);
                }
            }

            workbook = new Workbook(sourceDir + "example.xlsm");
            conns = workbook.DataConnections;
            foreach (ExternalConnection conn in conns)
            {
                if (conn is DBConnection dbConn)
                {
                    Console.WriteLine("Connection Info: " + dbConn.ConnectionInfo);
                    Console.WriteLine("Formula Definition: " + dbConn.PowerQueryFormula.FormulaDefinition);
                }
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


