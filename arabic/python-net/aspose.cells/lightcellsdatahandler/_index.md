---
title: LightCellsDataHandler الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 990
url: /ar/python-net/aspose.cells/lightcellsdatahandler/
is_root: false
---
##  LightCellsDataHandler الدرجة
يمثل معالج بيانات الخلايا لقراءة ملفات جداول البيانات الكبيرة في وضع الوزن الخفيف.



يكشف نوع LightCellsDataHandler الأعضاء التالية:

###  طُرق
| طريقة| وصف|
| :- | :- |
| [start_sheet(sheet)](/cells/ar/python-net/aspose.cells/lightcellsdatahandler/start_sheet/#Worksheet) | يبدأ في معالجة ورقة العمل.|
| [start_row(row_index)](/cells/ar/python-net/aspose.cells/lightcellsdatahandler/start_row/#int) | يستعد لمعالجة صف.|
| [process_row(row)](/cells/ar/python-net/aspose.cells/lightcellsdatahandler/process_row/#Row) | يبدأ في معالجة صف واحد.|
| [start_cell(column_index)](/cells/ar/python-net/aspose.cells/lightcellsdatahandler/start_cell/#int) | يستعد لمعالجة الخلية.|
| [process_cell(cell)](/cells/ar/python-net/aspose.cells/lightcellsdatahandler/process_cell/#Cell) | يبدأ في معالجة خلية واحدة.|



###  ملاحظات

عند قراءة مصنف بواسطة هذا الوضع ، سيتم التحقق من [LightCellsDataHandler.start_sheet(sheet)](/cells/ar/python-net/aspose.cells/lightcellsdatahandler/start_sheet) عند قراءة كل ورقة عمل في المصنف.
بالنسبة للورقة الواحدة ، إذا كانت قيمة [LightCellsDataHandler.start_sheet(sheet)](/cells/ar/python-net/aspose.cells/lightcellsdatahandler/start_sheet) صحيحة ، فسيتم فحص جميع بيانات وخصائص الصفوف / الخلايا في هذه الورقة
وتتم معالجتها من خلال تنفيذ هذه الواجهة. سيتم استدعاء [LightCellsDataHandler.start_row(row_index)](/cells/ar/python-net/aspose.cells/lightcellsdatahandler/start_row) لكل صف للتحقق مما إذا كان يلزم معالجته.
إذا احتاج صف إلى المعالجة ، فستتم قراءة خصائص هذا الصف أولاً ويمكن للمستخدم الوصول إلى خصائصه بحلول [LightCellsDataHandler.process_row(row)](/cells/ar/python-net/aspose.cells/lightcellsdatahandler/process_row).
إذا كانت خلايا الصف بحاجة إلى المعالجة أيضًا ، فيجب أن يعود [LightCellsDataHandler.process_row(row)](/cells/ar/python-net/aspose.cells/lightcellsdatahandler/process_row) صحيحًا ثم يكون [LightCellsDataHandler.start_cell(column_index)](/cells/ar/python-net/aspose.cells/lightcellsdatahandler/start_cell)
تم استدعاء كل خلية موجودة في هذا الصف للتحقق مما إذا كانت هناك خلية واحدة بحاجة إلى المعالجة.
ثم سيتم استدعاء [LightCellsDataHandler.process_cell(cell)](/cells/ar/python-net/aspose.cells/lightcellsdatahandler/process_cell) لمعالجة الخلية من خلال تنفيذ هذه الواجهة.

###  أنظر أيضا
* وحدة [aspose.cells](..)
