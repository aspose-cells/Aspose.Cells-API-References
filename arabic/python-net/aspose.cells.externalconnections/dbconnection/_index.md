---
title: DBConnection الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 30
url: /ar/python-net/aspose.cells.externalconnections/dbconnection/
is_root: false
---
##  DBConnection الدرجة
تحدد كافة الخصائص المقترنة باتصال بيانات خارجي ODBC أو OLE DB.



**ميراث:** [DBConnection](/cells/python-net/aspose.cells.externalconnections/dbconnection) → 
[ExternalConnection](/cells/ar/python-net/aspose.cells.externalconnections/externalconnection)



يكشف نوع DBConnection الأعضاء التالية:

###  ملكيات
| ملكية| وصف|
| :- | :- |
| [id](/cells/ar/python-net/aspose.cells.externalconnections/dbconnection/id) | يحصل على معرف الاتصال.|
| [power_query_formula](/cells/ar/python-net/aspose.cells.externalconnections/dbconnection/power_query_formula) | يحصل على تعريف صيغة استعلام الطاقة.|
| [type](/cells/ar/python-net/aspose.cells.externalconnections/dbconnection/type) | الحصول على أو تعيين نوع مصدر بيانات الاتصال الخارجي.|
| [source_file](/cells/ar/python-net/aspose.cells.externalconnections/dbconnection/source_file) | يُستخدم عندما يكون مصدر البيانات الخارجية مستندًا إلى الملف. عند الاتصال بمثل هذه البيانات<br/> فشل المصدر ، يحاول تطبيق جدول البيانات الاتصال مباشرة بهذا الملف. ربما<br/> معبرًا عنه في URI أو تدوين مسار الملف الخاص بالنظام.|
| [sso_id](/cells/ar/python-net/aspose.cells.externalconnections/dbconnection/sso_id) | معرّف للدخول الأحادي (SSO) يُستخدم للمصادقة بين وسيط<br/> خادم spreadsheetML ومصدر البيانات الخارجي.|
| [save_password](/cells/ar/python-net/aspose.cells.externalconnections/dbconnection/save_password) | صحيح إذا كان سيتم حفظ كلمة المرور كجزء من سلسلة الاتصال ؛ خلاف ذلك ، خطأ.|
| [save_data](/cells/ar/python-net/aspose.cells.externalconnections/dbconnection/save_data) | صواب إذا كان سيتم حفظ البيانات الخارجية التي تم جلبها عبر الاتصال لملء جدول<br/> مع المصنف خلاف ذلك ، خطأ.|
| [refresh_on_load](/cells/ar/python-net/aspose.cells.externalconnections/dbconnection/refresh_on_load) | صحيح إذا كان يجب تحديث هذا الاتصال عند فتح الملف ؛ خلاف ذلك ، خطأ.|
| [reconnection_method_type](/cells/ar/python-net/aspose.cells.externalconnections/dbconnection/reconnection_method_type) | يحدد ما يجب أن يفعله تطبيق جدول البيانات عند فشل الاتصال.<br/>القيمة الافتراضية هي ReConnectionMethodType.Required.|
| [reconnection_method](/cells/ar/python-net/aspose.cells.externalconnections/dbconnection/reconnection_method) | يحدد ما يجب أن يفعله تطبيق جدول البيانات عند فشل الاتصال.<br/>القيمة الافتراضية هي ReConnectionMethodType.Required.|
| [only_use_connection_file](/cells/ar/python-net/aspose.cells.externalconnections/dbconnection/only_use_connection_file) | يشير إلى ما إذا كان يجب أن يستخدم تطبيق جدول البيانات امتداد<br/> يشار إلى معلومات الاتصال في ملف الاتصال الخارجي بواسطة السمة odcFile<br/> عندما يتم تحديث الاتصال. إذا كان خطأ ، ثم تطبيق جدول البيانات<br/> يجب اتباع الإجراء المشار إليه بواسطة سمة إعادة الاتصال|
| [odc_file](/cells/ar/python-net/aspose.cells.externalconnections/dbconnection/odc_file) | يحدد المسار الكامل لملف الاتصال الخارجي الذي كان هذا الاتصال منه<br/> مخلوق. إذا فشل الاتصال أثناء محاولة تحديث البيانات ، وطريقة إعادة الاتصال = 1 ،<br/> ثم سيحاول تطبيق جدول البيانات مرة أخرى باستخدام معلومات من ملف الاتصال الخارجي<br/> بدلاً من كائن الاتصال المضمّن في المصنف.|
| [is_new](/cells/ar/python-net/aspose.cells.externalconnections/dbconnection/is_new) | صحيح إذا لم يتم تحديث الاتصال لأول مرة ؛ خلاف ذلك ، خطأ.<br/> يمكن أن تحدث هذه الحالة عندما يحفظ المستخدم الملف قبل أن ينتهي الاستعلام من العودة.|
| [name](/cells/ar/python-net/aspose.cells.externalconnections/dbconnection/name) | يحدد اسم الاتصال. يجب أن يكون لكل اتصال اسم فريد.|
| [keep_alive](/cells/ar/python-net/aspose.cells.externalconnections/dbconnection/keep_alive) | صحيح عندما يجب أن يبذل تطبيق جدول البيانات جهودًا للحفاظ على الاتصال<br/>يفتح. عندما يكون خطأ ، يجب أن يغلق التطبيق الاتصال بعد استرجاع ملف<br/> معلومة.|
| [refresh_internal](/cells/ar/python-net/aspose.cells.externalconnections/dbconnection/refresh_internal) | يحدد عدد الدقائق بين عمليات التحديث التلقائية للاتصال.|
| [connection_id](/cells/ar/python-net/aspose.cells.externalconnections/dbconnection/connection_id) | يحدد المعرف الفريد لهذا الاتصال.|
| [connection_description](/cells/ar/python-net/aspose.cells.externalconnections/dbconnection/connection_description) | يحدد وصف المستخدم لهذا الاتصال|
| [is_deleted](/cells/ar/python-net/aspose.cells.externalconnections/dbconnection/is_deleted) |يشير إلى ما إذا كان قد تم حذف اتصال المصنف المرتبط. صحيح إذا كان<br/> تم حذف الاتصال ؛ خلاف ذلك ، خطأ.|
| [credentials_method_type](/cells/ar/python-net/aspose.cells.externalconnections/dbconnection/credentials_method_type) | تحدد طريقة المصادقة التي سيتم استخدامها عند إنشاء الاتصال (أو إعادة تأسيسه).|
| [credentials](/cells/ar/python-net/aspose.cells.externalconnections/dbconnection/credentials) | تحدد طريقة المصادقة التي سيتم استخدامها عند إنشاء الاتصال (أو إعادة تأسيسه).|
| [background_refresh](/cells/ar/python-net/aspose.cells.externalconnections/dbconnection/background_refresh) | يشير إلى ما إذا كان يمكن تحديث الاتصال في الخلفية (بشكل غير متزامن).<br/>صحيح إذا كان الاستخدام المفضل للاتصال هو التحديث غير المتزامن في الخلفية ؛<br/> خطأ إذا كان الاستخدام المفضل للاتصال هو التحديث المتزامن في المقدمة.|
| [parameters](/cells/ar/python-net/aspose.cells.externalconnections/dbconnection/parameters) | الحصول على [ConnectionParameterCollection](/cells/ar/python-net/aspose.cells.externalconnections/connectionparametercollection) لاستعلام ويب أو ODBC.|
| [connection_info](/cells/ar/python-net/aspose.cells.externalconnections/dbconnection/connection_info) | يتم استخدام سلسلة معلومات الاتصال لإجراء اتصال بمصدر بيانات OLE DB أو ODBC.|
| [command_type](/cells/ar/python-net/aspose.cells.externalconnections/dbconnection/command_type) | تحدد نوع أمر OLE DB.<br/>1. يحدد الاستعلام اسم مكعب<br/>2. الاستعلام يحدد جملة SQL<br/>3. يحدد الاستعلام اسم جدول<br/>4. يحدد الاستعلام أن المعلومات الافتراضية قد تم تقديمها ، والأمر متروك للمزود في كيفية تفسيره.<br/> 5. الاستعلام ضد مزود بيانات القائمة على شبكة الإنترنت.|
| [command](/cells/ar/python-net/aspose.cells.externalconnections/dbconnection/command) | السلسلة التي تحتوي على أمر قاعدة البيانات لتمريرها إلى موفر البيانات API الذي سيقوم بذلك<br/> تتفاعل مع المصدر الخارجي من أجل استرداد البيانات|
| [sever_command](/cells/ar/python-net/aspose.cells.externalconnections/dbconnection/sever_command) |تعيين سلسلة نصية للأمر الثاني تستمر عندما يستند إلى خادم PivotTable<br/> حقول الصفحة قيد الاستخدام.<br/> بالنسبة لاتصالات ODBC ، يكون serverCommand عادةً استعلامًا أوسع من الأمر (no<br/>حيث يوجد شرط في السابق). بناءً على هذين الأمرين (Command and ServerCommand) ،<br/> يمكن ملء واجهة المستخدم للمعلمات وإنشاء استعلامات ذات معلمات|



###  أنظر أيضا
* وحدة [aspose.cells.externalconnections](..)
* فئة [ConnectionParameterCollection](/cells/ar/python-net/aspose.cells.externalconnections/connectionparametercollection)
* فئة [DBConnection](/cells/ar/python-net/aspose.cells.externalconnections/dbconnection)
* فئة [ExternalConnection](/cells/ar/python-net/aspose.cells.externalconnections/externalconnection)
