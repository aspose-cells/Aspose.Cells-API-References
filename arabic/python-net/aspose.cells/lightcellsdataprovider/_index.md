---
title: LightCellsDataProvider الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 1000
url: /ar/python-net/aspose.cells/lightcellsdataprovider/
is_root: false
---
##  LightCellsDataProvider الدرجة
يمثل مزود البيانات لحفظ ملفات جداول البيانات الكبيرة في وضع الوزن الخفيف.



يكشف نوع LightCellsDataProvider الأعضاء التالية:

###  طُرق
| طريقة| وصف|
| :- | :- |
| [start_sheet(sheet_index)](/cells/ar/python-net/aspose.cells/lightcellsdataprovider/start_sheet/#int) | يبدأ في حفظ ورقة العمل.|
| [next_row()](/cells/ar/python-net/aspose.cells/lightcellsdataprovider/next_row/#) | يحصل على الصف التالي ليتم حفظه.|
| [start_row(row)](/cells/ar/python-net/aspose.cells/lightcellsdataprovider/start_row/#Row) | يبدأ في حفظ بيانات صف واحد.|
| [next_cell()](/cells/ar/python-net/aspose.cells/lightcellsdataprovider/next_cell/#) | يحصل على الخلية التالية ليتم حفظها.|
| [start_cell(cell)](/cells/ar/python-net/aspose.cells/lightcellsdataprovider/start_cell/#Cell) | يبدأ في حفظ بيانات خلية واحدة.|
| [is_gather_string()](/cells/ar/python-net/aspose.cells/lightcellsdataprovider/is_gather_string/#) |للتحقق مما إذا كانت قيمة السلسلة الحالية للخلية بحاجة إلى أن يتم تجميعها في تجمع عمومي.|



###  ملاحظات

عند حفظ مصنف بواسطة هذا الوضع ، سيتم التحقق من [LightCellsDataProvider.start_sheet(sheet_index)](/cells/ar/python-net/aspose.cells/lightcellsdataprovider/start_sheet) عند حفظ كل ورقة عمل في المصنف.
بالنسبة للورقة الواحدة ، إذا كانت قيمة [LightCellsDataProvider.start_sheet(sheet_index)](/cells/ar/python-net/aspose.cells/lightcellsdataprovider/start_sheet) صحيحة ، فسيتم حفظ جميع بيانات وخصائص الصفوف / الخلايا في هذه الورقة
سيتم توفيره من خلال تنفيذ هذه الواجهة. في المقام الأول ، سيتم استدعاء [LightCellsDataProvider.next_row()](/cells/ar/python-net/aspose.cells/lightcellsdataprovider/next_row) للحصول على فهرس الصف التالي ليتم حفظه.
إذا تم إرجاع فهرس صف صالح (يجب أن يكون فهرس الصف بترتيب تصاعدي حتى يتم حفظ الصفوف) ،
ثم سيتم توفير كائن صف يمثل هذا الصف للتنفيذ لتعيين خصائصه بواسطة [LightCellsDataProvider.start_row(row)](/cells/ar/python-net/aspose.cells/lightcellsdataprovider/start_row).
لصف واحد ، سيتم فحص [LightCellsDataProvider.next_cell()](/cells/ar/python-net/aspose.cells/lightcellsdataprovider/next_cell) أولاً. إذا تم إرجاع فهرس عمود صالح (يجب أن يكون فهرس العمود بترتيب تصاعدي لجميع الخلايا في صف واحد ليتم حفظه) ،
ثم سيتم توفير عنصر Cell يمثل هذه الخلية للتنفيذ لتعيين بياناتها وخصائصها بواسطة [LightCellsDataProvider.start_cell(cell)](/cells/ar/python-net/aspose.cells/lightcellsdataprovider/start_cell).
بعد تعيين بيانات هذه الخلية ، سيتم حفظ هذه الخلية مباشرة في ملف جدول البيانات الذي تم إنشاؤه وسيتم فحص الخلية التالية ومعالجتها.

###  أنظر أيضا
* وحدة [aspose.cells](..)
