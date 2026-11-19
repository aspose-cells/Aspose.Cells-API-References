---
title: "LightCellsDataHandler"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل معالج بيانات الخلايا لقراءة ملفات جداول البيانات الكبيرة في وضع خفيف الوزن."
type: docs
url: /ar/java/com.aspose.cells/lightcellsdatahandler/
---
```
public interface LightCellsDataHandler
```

يمثل معالج بيانات الخلايا لقراءة ملفات جداول البيانات الكبيرة في وضع خفيف الوزن.

**Remarks**

عند قراءة مصنف بهذه الطريقة، سيتم فحص [startSheet(Worksheet)](../../com.aspose.cells/lightcellsdatahandler\#startSheet-Worksheet-) عند قراءة كل ورقة عمل في المصنف. لورقة واحدة، إذا أعطى [startSheet(Worksheet)](../../com.aspose.cells/lightcellsdatahandler\#startSheet-Worksheet-) قيمة true، فسيتم فحص جميع البيانات وخصائص الصفوف/الخلايا في هذه الورقة ومعالجتها بواسطة تنفيذ هذه الواجهة. لكل صف، سيتم استدعاء [startRow(int)](../../com.aspose.cells/lightcellsdatahandler\#startRow-int-) للتحقق مما إذا كان يحتاج إلى المعالجة. إذا كان الصف يحتاج إلى المعالجة، ستُقرأ خصائص هذا الصف أولاً ويمكن للمستخدم الوصول إلى خصائصه عبر [processRow(Row)](../../com.aspose.cells/lightcellsdatahandler\#processRow-Row-). إذا كانت خلايا الصف تحتاج إلى المعالجة أيضًا، يجب أن تُعيد [processRow(Row)](../../com.aspose.cells/lightcellsdatahandler\#processRow-Row-) قيمة true ثم سيتم استدعاء [startCell(int)](../../com.aspose.cells/lightcellsdatahandler\#startCell-int-) لكل خلية موجودة في هذا الصف للتحقق مما إذا كانت الخلية تحتاج إلى المعالجة. إذا كانت الخلية تحتاج إلى المعالجة، سيتم استدعاء [processCell(Cell)](../../com.aspose.cells/lightcellsdatahandler\#processCell-Cell-) لمعالجة الخلية بواسطة تنفيذ هذه الواجهة.

يرجى ملاحظة أن المستخدم يجب أن يتعامل فقط مع القيم والخصائص لكائن Row/Cell الحالي المقدم بواسطة الطريقة المقابلة. نظرًا لأن بيانات الخلايا تُقرأ من ملف القالب بطريقة تدفقية، قد يتم إعادة ضبط/تحديث معظم الكائنات الأخرى لاحقًا بعد تحميل بيانات الخلايا. لذلك عندما يقوم المستخدم بالتعامل مع كائنات أخرى في هذا التنفيذ، قد لا تؤثر تلك العمليات على الكائنات الموجودة في المصنف. بل والأسوأ، قد تتسبب تلك العمليات في بيانات غير متسقة في المصنف ثم تؤدي إلى مشكلة أو استثناء غير متوقع لاحقًا. لذا، بالنسبة لجميع الكائنات الأخرى مثل الأشكال، عرض الأعمدة والأنماط، التنسيقات الشرطية، ... إلخ، يرجى عدم التعامل معها في أي من طرق هذا التنفيذ. بدلاً من ذلك، يرجى إدارتها بعد إنشاء المصنف.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [processCell(Cell cell)](#processCell-com.aspose.cells.Cell-) | يبدأ معالجة خلية واحدة. |
| [processRow(Row row)](#processRow-com.aspose.cells.Row-) | يبدأ معالجة صف واحد. |
| [startCell(int columnIndex)](#startCell-int-) | يستعد لمعالجة خلية. |
| [startRow(int rowIndex)](#startRow-int-) | يستعد لمعالجة صف. |
| [startSheet(Worksheet sheet)](#startSheet-com.aspose.cells.Worksheet-) | يبدأ معالجة ورقة عمل. |
### processCell(Cell cell) {#processCell-com.aspose.cells.Cell-}
```
public abstract boolean processCell(Cell cell)
```


يبدأ معالجة خلية واحدة.

**Remarks**

سيتم استدعاؤه بعد قراءة بيانات خلية واحدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| cell | [Cell](../../com.aspose.cells/cell) | كائن الخلية الذي يتم معالجته حاليًا |

**Returns:**
منطقي - ما إذا كان يجب الاحتفاظ بهذه الخلية في نموذج الخلايا للورقة الحالية. عادةً يجب أن يكون false بحيث لا يتم الاحتفاظ بجميع الخلايا في الذاكرة بعد معالجتها وبالتالي يتم توفير الذاكرة. لبعض الأغراض الخاصة مثل الحاجة إلى الوصول إلى بعض الخلايا لاحقًا بعد معالجة المصنف بالكامل، يمكن للمستخدم جعل هذه الطريقة تُعيد true للاحتفاظ بتلك الخلايا الخاصة في نموذج Cells والوصول إليها لاحقًا عبر واجهات برمجة التطبيقات مثل Cells[row, column]. ومع ذلك، سيؤدي الاحتفاظ ببيانات الخلايا في نموذج Cells إلى استهلاك المزيد من الذاكرة وإذا تم الاحتفاظ بجميع الخلايا فإن قراءة ملف القالب في وضع LightCells ستصبح مماثلة للقراءة بالطريقة العادية.
### processRow(Row row) {#processRow-com.aspose.cells.Row-}
```
public abstract boolean processRow(Row row)
```


يبدأ معالجة صف واحد.

**Remarks**

سيتم استدعاؤه بعد قراءة خصائص الصف مثل الارتفاع، النمط، ... إلخ. ومع ذلك، لم تُقرأ خلايا هذا الصف بعد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| row | [Row](../../com.aspose.cells/row) | كائن الصف الذي يتم معالجته حاليًا. |

**Returns:**
منطقي - ما إذا كانت خلايا هذا الصف تحتاج إلى المعالجة. false لتجاهل جميع الخلايا في هذا الصف.
### startCell(int columnIndex) {#startCell-int-}
```
public abstract boolean startCell(int columnIndex)
```


يستعد لمعالجة خلية.

**Remarks**

سيتم استدعاؤه عند الوصول إلى خلية موجودة في الصف الحالي. الصف الحالي هو الصف الذي تم استدعاؤه آخر مرة بواسطة [processRow(Row)](../../com.aspose.cells/lightcellsdatahandler\#processRow-Row-).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| columnIndex | int | فهرس العمود للخلية التي سيتم معالجتها |

**Returns:**
boolean - ما إذا كانت هذه الخلية تحتاج إلى المعالجة. false لتجاهل الخلية والتحقق من التالية حتى الوصول إلى نهاية بيانات الخلايا في الصف الحالي
### startRow(int rowIndex) {#startRow-int-}
```
public abstract boolean startRow(int rowIndex)
```


يستعد لمعالجة صف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rowIndex | int | فهرس الصف التالي الذي سيتم معالجته |

**Returns:**
boolean - ما إذا كان هذا الصف (الخصائص أو بيانات الخلايا) يحتاج إلى المعالجة. false لتجاهل هذا الصف وخلاياه والتحقق من الصف التالي.
### startSheet(Worksheet sheet) {#startSheet-com.aspose.cells.Worksheet-}
```
public abstract boolean startSheet(Worksheet sheet)
```


يبدأ معالجة ورقة عمل.

**Remarks**

سيتم استدعاؤه قبل قراءة بيانات الخلايا في ورقة العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sheet | [Worksheet](../../com.aspose.cells/worksheet) | ورقة العمل التي سيتم قراءة بيانات الخلايا منها. |

**Returns:**
boolean - ما إذا كانت بيانات خلايا هذه الورقة تحتاج إلى المعالجة. false لتجاهل هذه الورقة.
