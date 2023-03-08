---
title: VbaProjectReferenceCollection الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 50
url: /ar/python-net/aspose.cells.vba/vbaprojectreferencecollection/
is_root: false
---
##  VbaProjectReferenceCollection الدرجة
يمثل جميع مراجع مشروع VBA.



يكشف نوع VbaProjectReferenceCollection الأعضاء التالية:

###  ملكيات
| ملكية| وصف|
| :- | :- |
| [capacity](/cells/ar/python-net/aspose.cells.vba/vbaprojectreferencecollection/capacity) | الحصول على أو تحديد عدد العناصر التي يمكن أن تحتويها قائمة الصفيف.|


###  طُرق
| طريقة| وصف|
| :- | :- |
| [copy_to(array)](/cells/ar/python-net/aspose.cells.vba/vbaprojectreferencecollection/copy_to/#list) | ينسخ قائمة المصفوفات بأكملها إلى قائمة مصفوفة متوافقة أحادية البعد ، بدءًا من بداية قائمة الصفيف الهدف.|
| [copy_to(index, array, array_index, count)](/cells/ar/python-net/aspose.cells.vba/vbaprojectreferencecollection/copy_to/#int-list-int-int) | ينسخ نطاقًا من العناصر من قائمة المصفوفة إلى قائمة مصفوفة أحادية البعد متوافقة ، بدءًا من الفهرس المحدد لقائمة الصفيف الهدف.|
| [index_of(item, index)](/cells/ar/python-net/aspose.cells.vba/vbaprojectreferencecollection/index_of/#VbaProjectReference-int) | البحث عن الكائن المحدد وإرجاع الفهرس الصفري للتواجد الأول ضمن نطاق العناصر في قائمة الصفيف الذي يمتد من الفهرس المحدد إلى العنصر الأخير.|
| [index_of(item, index, count)](/cells/ar/python-net/aspose.cells.vba/vbaprojectreferencecollection/index_of/#VbaProjectReference-int-int) | البحث عن الكائن المحدد وإرجاع الفهرس الصفري للتواجد الأول ضمن نطاق العناصر في قائمة الصفيف الذي يبدأ بالفهرس المحدد ويحتوي على عدد محدد من العناصر.|
| [last_index_of(item)](/cells/ar/python-net/aspose.cells.vba/vbaprojectreferencecollection/last_index_of/#VbaProjectReference) | البحث عن الكائن المحدد وإرجاع الفهرس الصفري للتواجد الأخير ضمن قائمة الصفيف بأكملها.|
| [last_index_of(item, index)](/cells/ar/python-net/aspose.cells.vba/vbaprojectreferencecollection/last_index_of/#VbaProjectReference-int) |يبحث عن الكائن المحدد ويعيد الفهرس الصفري للتواجد الأخير ضمن نطاق العناصر في قائمة الصفيف الذي يمتد من العنصر الأول إلى الفهرس المحدد.|
| [last_index_of(item, index, count)](/cells/ar/python-net/aspose.cells.vba/vbaprojectreferencecollection/last_index_of/#VbaProjectReference-int-int) | يبحث عن الكائن المحدد ويعيد الفهرس الصفري للتواجد الأخير ضمن نطاق العناصر في قائمة الصفيف التي تحتوي على عدد محدد من العناصر وتنتهي عند الفهرس المحدد.|
| [add_registered_reference(name, libid)](/cells/ar/python-net/aspose.cells.vba/vbaprojectreferencecollection/add_registered_reference/#str-str) | قم بإضافة مرجع إلى مكتبة نوع التنفيذ.|
| [add_control_refrernce(name, libid, twiddledlibid, extended_libid)](/cells/ar/python-net/aspose.cells.vba/vbaprojectreferencecollection/add_control_refrernce/#str-str-str-str) | أضف مرجعًا إلى مكتبة نوع ملفوفة ومكتبة النوع الموسعة الخاصة بها.|
| [add_project_refrernce(name, absolute_libid, relative_libid)](/cells/ar/python-net/aspose.cells.vba/vbaprojectreferencecollection/add_project_refrernce/#str-str-str) | يضيف مرجعًا إلى مشروع VBA خارجي.|
| [binary_search(item)](/cells/ar/python-net/aspose.cells.vba/vbaprojectreferencecollection/binary_search/#VbaProjectReference) | يبحث في قائمة الصفيف التي تم فرزها بالكامل عن عنصر باستخدام المقارنة الافتراضية ويعيد فهرس العنصر على أساس الصفر.|



###  مثال

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
#  Init VBA project.
vbaProject = workbook.vba_project
#  Add vba project reference
vbaProject.references.add_registered_reference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation")
# Saving the Excel file
workbook.save("book1.xlsm")

```

###  أنظر أيضا
* وحدة [aspose.cells.vba](..)
