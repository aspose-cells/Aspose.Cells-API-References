---
title: ConnectionParameter الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 10
url: /ar/python-net/aspose.cells.externalconnections/connectionparameter/
is_root: false
---
##  ConnectionParameter الدرجة
يحدد خصائص حول أي معلمات مستخدمة مع اتصالات البيانات الخارجية
المعلمات صالحة لـ ODBC واستعلامات الويب.



يكشف نوع ConnectionParameter الأعضاء التالية:

###  ملكيات
| ملكية| وصف|
| :- | :- |
| [sql_type](/cells/ar/python-net/aspose.cells.externalconnections/connectionparameter/sql_type) | نوع بيانات SQL للمعلمة. صالح فقط لمصادر ODBC.|
| [refresh_on_change](/cells/ar/python-net/aspose.cells.externalconnections/connectionparameter/refresh_on_change) | علامة تشير إلى ما إذا كان يجب تحديث الاستعلام تلقائيًا عند تحديث محتويات ملف<br/> الخلية التي توفر تغيير قيمة المعلمة. إذا كان هذا صحيحًا ، فسيتم تحديث البيانات الخارجية<br/> باستخدام قيمة المعلمة الجديدة في كل مرة يحدث فيها تغيير. إذا كانت خاطئة ، ثم البيانات الخارجية<br/> يتم تحديثه فقط عند طلب المستخدم ، أو تحديث بعض مشغلات الأحداث الأخرى (على سبيل المثال ، تم فتح المصنف).|
| [prompt](/cells/ar/python-net/aspose.cells.externalconnections/connectionparameter/prompt) | سلسلة مطالبة للمعلمة. يتم تقديمها إلى مستخدم جدول البيانات مع واجهة مستخدم الإدخال<br/> لتجميع قيمة المعلمة قبل تحديث البيانات الخارجية. تستخدم فقط عندما<br/>نوع المعامل = موجه.|
| [type](/cells/ar/python-net/aspose.cells.externalconnections/connectionparameter/type) | نوع المعلمة المستخدمة.<br/> إذا كانت المعلمة نوع = قيمة ، فإن القيمة من منطقية ، مزدوجة ، عدد صحيح ،<br/> أو السلسلة. في هذه الحالة ، من المتوقع أن يكون واحدًا فقط من<br/> سيتم تحديد {منطقية أو مزدوجة أو صحيحة أو سلسلة}.|
| [name](/cells/ar/python-net/aspose.cells.externalconnections/connectionparameter/name) | اسم المعامل.|
| [cell_reference](/cells/ar/python-net/aspose.cells.externalconnections/connectionparameter/cell_reference) | مرجع Cell يشير إلى قيمة الخانة التي سيتم استخدامها لمعامل الاستعلام. يُستخدم فقط عندما تكون معلمة نوع الخلية.|
| [value](/cells/ar/python-net/aspose.cells.externalconnections/connectionparameter/value) | قيمة عددية غير صحيحة أو قيمة عدد صحيح أو قيمة سلسلة أو قيمة منطقية<br/> لاستخدامها كمعامل طلب البحث. يستخدم فقط عندما تكون قيمة parameterType هي القيمة.|



###  أنظر أيضا
* وحدة [aspose.cells.externalconnections](..)
