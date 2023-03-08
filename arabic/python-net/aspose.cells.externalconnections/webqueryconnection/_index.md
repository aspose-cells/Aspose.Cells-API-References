---
title: WebQueryConnection الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 70
url: /ar/python-net/aspose.cells.externalconnections/webqueryconnection/
is_root: false
---
##  WebQueryConnection الدرجة
 يحدد خصائص مصدر استعلام ويب. سيقوم استعلام الويب باسترداد البيانات من جداول HTML ،
 ويمكن أيضًا توفير معلمات HTTP "Get" ليتم معالجتها بواسطة خادم الويب في إنشاء HTML بواسطة
بما في ذلك المعلمات وعناصر المعلمة.



**ميراث:** [WebQueryConnection](/cells/python-net/aspose.cells.externalconnections/webqueryconnection) → 
[ExternalConnection](/cells/ar/python-net/aspose.cells.externalconnections/externalconnection)



يكشف نوع WebQueryConnection الأعضاء التالية:

###  ملكيات
| ملكية| وصف|
| :- | :- |
| [id](/cells/ar/python-net/aspose.cells.externalconnections/webqueryconnection/id) | يحصل على معرف الاتصال.|
| [power_query_formula](/cells/ar/python-net/aspose.cells.externalconnections/webqueryconnection/power_query_formula) | يحصل على تعريف صيغة استعلام الطاقة.|
| [type](/cells/ar/python-net/aspose.cells.externalconnections/webqueryconnection/type) | الحصول على أو تعيين نوع مصدر بيانات الاتصال الخارجي.|
| [source_file](/cells/ar/python-net/aspose.cells.externalconnections/webqueryconnection/source_file) | يُستخدم عندما يكون مصدر البيانات الخارجية مستندًا إلى الملف. عند الاتصال بمثل هذه البيانات<br/> فشل المصدر ، يحاول تطبيق جدول البيانات الاتصال مباشرة بهذا الملف. ربما<br/> معبرًا عنه في URI أو تدوين مسار الملف الخاص بالنظام.|
| [sso_id](/cells/ar/python-net/aspose.cells.externalconnections/webqueryconnection/sso_id) | معرّف للدخول الأحادي (SSO) يُستخدم للمصادقة بين وسيط<br/>خادم spreadsheetML ومصدر البيانات الخارجي.|
| [save_password](/cells/ar/python-net/aspose.cells.externalconnections/webqueryconnection/save_password) |صحيح إذا كان سيتم حفظ كلمة المرور كجزء من سلسلة الاتصال ؛ خلاف ذلك ، خطأ.|
| [save_data](/cells/ar/python-net/aspose.cells.externalconnections/webqueryconnection/save_data) | صواب إذا كان سيتم حفظ البيانات الخارجية التي تم جلبها عبر الاتصال لملء جدول<br/> مع المصنف خلاف ذلك ، خطأ.|
| [refresh_on_load](/cells/ar/python-net/aspose.cells.externalconnections/webqueryconnection/refresh_on_load) | صحيح إذا كان يجب تحديث هذا الاتصال عند فتح الملف ؛ خلاف ذلك ، خطأ.|
| [reconnection_method_type](/cells/ar/python-net/aspose.cells.externalconnections/webqueryconnection/reconnection_method_type) | يحدد ما يجب أن يفعله تطبيق جدول البيانات عند فشل الاتصال.<br/> القيمة الافتراضية هي ReConnectionMethodType.Required.|
| [reconnection_method](/cells/ar/python-net/aspose.cells.externalconnections/webqueryconnection/reconnection_method) | يحدد ما يجب أن يفعله تطبيق جدول البيانات عند فشل الاتصال.<br/> القيمة الافتراضية هي ReConnectionMethodType.Required.|
| [only_use_connection_file](/cells/ar/python-net/aspose.cells.externalconnections/webqueryconnection/only_use_connection_file) | يشير إلى ما إذا كان يجب أن يستخدم تطبيق جدول البيانات امتداد<br/> يشار إلى معلومات الاتصال في ملف الاتصال الخارجي بواسطة السمة odcFile<br/> عندما يتم تحديث الاتصال. إذا كان خطأ ، ثم تطبيق جدول البيانات<br/> يجب اتباع الإجراء المشار إليه بواسطة سمة إعادة الاتصال|
| [odc_file](/cells/ar/python-net/aspose.cells.externalconnections/webqueryconnection/odc_file) | يحدد المسار الكامل لملف الاتصال الخارجي الذي كان هذا الاتصال منه<br/> مخلوق. إذا فشل الاتصال أثناء محاولة تحديث البيانات ، وطريقة إعادة الاتصال = 1 ،<br/> ثم سيحاول تطبيق جدول البيانات مرة أخرى باستخدام معلومات من ملف الاتصال الخارجي<br/> بدلاً من كائن الاتصال المضمّن في المصنف.|
| [is_new](/cells/ar/python-net/aspose.cells.externalconnections/webqueryconnection/is_new) | صحيح إذا لم يتم تحديث الاتصال لأول مرة ؛ خلاف ذلك ، خطأ.<br/> يمكن أن تحدث هذه الحالة عندما يحفظ المستخدم الملف قبل أن ينتهي الاستعلام من العودة.|
| [name](/cells/ar/python-net/aspose.cells.externalconnections/webqueryconnection/name) | يحدد اسم الاتصال. يجب أن يكون لكل اتصال اسم فريد.|
| [keep_alive](/cells/ar/python-net/aspose.cells.externalconnections/webqueryconnection/keep_alive) | صحيح عندما يجب أن يبذل تطبيق جدول البيانات جهودًا للحفاظ على الاتصال<br/> يفتح. عندما يكون خطأ ، يجب أن يغلق التطبيق الاتصال بعد استرجاع ملف<br/> معلومة.|
| [refresh_internal](/cells/ar/python-net/aspose.cells.externalconnections/webqueryconnection/refresh_internal) | يحدد عدد الدقائق بين عمليات التحديث التلقائية للاتصال.|
| [connection_id](/cells/ar/python-net/aspose.cells.externalconnections/webqueryconnection/connection_id) | يحدد المعرف الفريد لهذا الاتصال.|
| [connection_description](/cells/ar/python-net/aspose.cells.externalconnections/webqueryconnection/connection_description) | يحدد وصف المستخدم لهذا الاتصال|
| [is_deleted](/cells/ar/python-net/aspose.cells.externalconnections/webqueryconnection/is_deleted) | يشير إلى ما إذا كان قد تم حذف اتصال المصنف المرتبط. صحيح إذا كان<br/> تم حذف الاتصال ؛ خلاف ذلك ، خطأ.|
| [credentials_method_type](/cells/ar/python-net/aspose.cells.externalconnections/webqueryconnection/credentials_method_type) | تحدد طريقة المصادقة التي سيتم استخدامها عند إنشاء الاتصال (أو إعادة تأسيسه).|
| [credentials](/cells/ar/python-net/aspose.cells.externalconnections/webqueryconnection/credentials) | تحدد طريقة المصادقة التي سيتم استخدامها عند إنشاء الاتصال (أو إعادة تأسيسه).|
| [background_refresh](/cells/ar/python-net/aspose.cells.externalconnections/webqueryconnection/background_refresh) | يشير إلى ما إذا كان يمكن تحديث الاتصال في الخلفية (بشكل غير متزامن).<br/> صحيح إذا كان الاستخدام المفضل للاتصال هو التحديث غير المتزامن في الخلفية ؛<br/>خطأ إذا كان الاستخدام المفضل للاتصال هو التحديث المتزامن في المقدمة.|
| [parameters](/cells/ar/python-net/aspose.cells.externalconnections/webqueryconnection/parameters) | الحصول على [ConnectionParameterCollection](/cells/ar/python-net/aspose.cells.externalconnections/connectionparametercollection) لاستعلام ويب أو ODBC.|
| [is_xml](/cells/ar/python-net/aspose.cells.externalconnections/webqueryconnection/is_xml) | صواب إذا كان مصدر استعلام الويب هو XML (مقابل HTML) ، وإلا فهو خطأ.|
| [is_xl97](/cells/ar/python-net/aspose.cells.externalconnections/webqueryconnection/is_xl97) | توجد هذه العلامة للتوافق مع ملفات جداول البيانات الحالية القديمة ، وتم تعيينها<br/>إلى true إذا تم إنشاء استعلام الويب هذا في Microsoft Excel 97.<br/> هذه سمة اختيارية يمكن تجاهلها.|
| [is_xl2000](/cells/ar/python-net/aspose.cells.externalconnections/webqueryconnection/is_xl2000) | توجد هذه العلامة للتوافق مع ملفات جداول البيانات الحالية القديمة ، وتم تعيينها<br/>إلى true إذا تم تحديث استعلام الويب هذا في تطبيق جدول بيانات أحدث من أو يساوي<br/>إلى Microsoft Excel 2000.<br/> هذه سمة اختيارية يمكن تجاهلها.|
| [url](/cells/ar/python-net/aspose.cells.externalconnections/webqueryconnection/url) | URL المطلوب استخدامه لتحديث البيانات الخارجية.|
| [is_text_dates](/cells/ar/python-net/aspose.cells.externalconnections/webqueryconnection/is_text_dates) | علامة تشير إلى ما إذا كان يجب استيراد التواريخ إلى خلايا في ورقة العمل كنص وليس كتواريخ.|
| [is_xml_source_data](/cells/ar/python-net/aspose.cells.externalconnections/webqueryconnection/is_xml_source_data) | إشارة تشير إلى أنه يجب استقبال بيانات مصدر XML بدلاً من جدول HTML نفسه.|
| [post](/cells/ar/python-net/aspose.cells.externalconnections/webqueryconnection/post) | إرجاع أو تعيين السلسلة المستخدمة مع طريقة النشر لإدخال البيانات في خادم ويب<br/> لإرجاع البيانات من استعلام الويب.|
| [is_parse_pre](/cells/ar/python-net/aspose.cells.externalconnections/webqueryconnection/is_parse_pre) |علامة تشير إلى ما إذا كانت البيانات المضمنة في علامات PRE HTML في صفحة الويب هي أم لا<br/> يتم توزيعها في أعمدة عند استيراد الصفحة إلى جدول استعلام.|
| [is_html_tables](/cells/ar/python-net/aspose.cells.externalconnections/webqueryconnection/is_html_tables) | إشارة تشير إلى ما إذا كان يجب أن تعمل استعلامات الويب على جداول HTML فقط.|
| [html_format](/cells/ar/python-net/aspose.cells.externalconnections/webqueryconnection/html_format) | كيفية التعامل مع التنسيق من المصدر HTML عند إحضار بيانات استعلام الويب في ملف<br/> ورقة عمل. ذات صلة عندما تكون بيانات المصدر صحيحة.|
| [is_same_settings](/cells/ar/python-net/aspose.cells.externalconnections/webqueryconnection/is_same_settings) | علامة تشير إلى ما إذا كان سيتم تحليل كل الجداول داخل كتلة PRE بنفس إعدادات العرض<br/> كالصف الأول.|
| [edit_web_page](/cells/ar/python-net/aspose.cells.externalconnections/webqueryconnection/edit_web_page) | عنوان URL لصفحة الويب التي تواجه المستخدم والتي تعرض بيانات استعلام الويب. عنوان URL هذا مستمر<br/>في حالة إعادة توجيه sourceData = "true" وعنوان url للإشارة إلى ملف XML.<br/>ثم يمكن عرض الصفحة التي تواجه المستخدم في واجهة المستخدم ، ويمكن استرداد بيانات XML<br/> خلف الكواليس.|
| [edit_page](/cells/ar/python-net/aspose.cells.externalconnections/webqueryconnection/edit_page) | عنوان URL لصفحة الويب التي تواجه المستخدم والتي تعرض بيانات استعلام الويب. عنوان URL هذا مستمر<br/>في حالة إعادة توجيه sourceData = "true" وعنوان url للإشارة إلى ملف XML.<br/>ثم يمكن عرض الصفحة التي تواجه المستخدم في واجهة المستخدم ، ويمكن استرداد بيانات XML<br/> خلف الكواليس.|
| [is_consecutive](/cells/ar/python-net/aspose.cells.externalconnections/webqueryconnection/is_consecutive) | علامة تشير إلى ما إذا كان يجب معاملة المحددات المتتالية كمحدد واحد فقط.|



###  أنظر أيضا
* وحدة [aspose.cells.externalconnections](..)
* فئة [ConnectionParameterCollection](/cells/ar/python-net/aspose.cells.externalconnections/connectionparametercollection)
* فئة [ExternalConnection](/cells/ar/python-net/aspose.cells.externalconnections/externalconnection)
* فئة [WebQueryConnection](/cells/ar/python-net/aspose.cells.externalconnections/webqueryconnection)
