---
title: "GridHtmlSaveOptions"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل الخيارات لحفظ ملف html."
type: docs
url: /ar/java/com.aspose.gridweb/gridhtmlsaveoptions/
---

**Inheritance:**
java.lang.Object، [com.aspose.gridweb.GridSaveOptions](../../com.aspose.gridweb/gridsaveoptions)
```
public class GridHtmlSaveOptions extends GridSaveOptions
```

يمثل الخيارات لحفظ ملف html.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [GridHtmlSaveOptions()](#GridHtmlSaveOptions--) | ينشئ خيارات لحفظ ملف html. |
| [GridHtmlSaveOptions(int format)](#GridHtmlSaveOptions-int-) | ينشئ خيارات لحفظ ملف htm. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAttachedFilesDirectory()](#getAttachedFilesDirectory--) | الدليل الذي سيتم حفظ الملفات المرفقة فيه. |
| [getAttachedFilesUrlPrefix()](#getAttachedFilesUrlPrefix--) | حدد بادئة URL للملفات المرفقة مثل الصورة في ملف HTML. |
| [getCachedFileFolder()](#getCachedFileFolder--) | مجلد الملفات المؤقت يُستخدم لتخزين بعض البيانات الكبيرة. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | اجعل دفتر العمل فارغًا بعد حفظ الملف. |
| [getCreateDirectory()](#getCreateDirectory--) | إذا كان صحيحًا ولم يكن الدليل موجودًا، فسيتم إنشاء الدليل تلقائيًا قبل حفظ الملف. |
| [getDefaultFontName()](#getDefaultFontName--) | حدد اسم الخط الافتراضي لتصدير HTML، سيتم استخدام الخط الافتراضي عندما لا يكون خط النمط موجودًا، إذا كانت هذه الخاصية فارغة (null)، سيستخدم Aspose.Cells خطًا عالميًا يملك نفس عائلة الخط الأصلي، القيمة الافتراضية هي null. |
| [getEncoding()](#getEncoding--) | إذا لم يتم تحديده، استخدم Encoding.UTF8 كنمط الترميز الافتراضي. |
| [getExportActiveWorksheetOnly()](#getExportActiveWorksheetOnly--) | يشير إلى ما إذا كان يتم تصدير المصنف بالكامل إلى ملف html. |
| [getExportArea()](#getExportArea--) | يحصل على نطاق الخلايا (CellArea) المُصدَّر للورقة النشطة الحالية. |
| [getExportGridLines()](#getExportGridLines--) | الإشارة إلى ما إذا كان يتم تصدير خطوط الشبكة. القيمة الافتراضية هي false. |
| [getExportHeadings()](#getExportHeadings--) | يشير إلى ما إذا كان يتم تصدير العناوين عند حفظ الملف إلى html. القيمة الافتراضية هي false. |
| [getExportHiddenWorksheet()](#getExportHiddenWorksheet--) | الإشارة إلى ما إذا كان يتم تصدير محتوى ورقة العمل المخفي. القيمة الافتراضية هي true. |
| [getExportImagesAsBase64()](#getExportImagesAsBase64--) | يحدد ما إذا كانت الصور تُحفظ بتنسيق Base64 إلى HTML أو MHTML أو EPUB. |
| [getExportPrintAreaOnly()](#getExportPrintAreaOnly--) | يحدد ما إذا كان يتم تصدير منطقة الطباعة فقط إلى ملف HTML. |
| [getExportSingleTab()](#getExportSingleTab--) | يحدد ما إذا كان يتم تصدير علامة التبويب الوحيدة عندما يحتوي الملف على ورقة عمل واحدة فقط. |
| [getMergeAreas()](#getMergeAreas--) | يحدد ما إذا كان يتم دمج مناطق التنسيق الشرطي والتحقق قبل حفظ الملف. |
| [getPageTitle()](#getPageTitle--) | عنوان صفحة HTML. |
|  | [getParseHtmlTagInCell()](#getParseHtmlTagInCell--) | تحليل علامة html في الخلية، مثل |

، كقيمة خلية، أو كعلامة html، القيمة الافتراضية هي true |
| [getPresentationPreference()](#getPresentationPreference--) | الإشارة إلى ما إذا كان ملف html أو mht هو تفضيل العرض. القيمة الافتراضية هي false. إذا كنت تريد الحصول على عرض أكثر جمالًا، يرجى ضبط القيمة إلى true. |
| [getRefreshChartCache()](#getRefreshChartCache--) | يشير إلى ما إذا كان يتم تحديث بيانات مخزن مؤقت المخطط |
| [getSaveFormat()](#getSaveFormat--) | يحصل على صيغة حفظ الملف. |
| [getSortNames()](#getSortNames--) | يحدد ما إذا كان يتم فرز الأسماء المعرفة قبل حفظ الملف. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | يحدد ما إذا كان يتم التحقق من صحة الخلايا المدمجة قبل حفظ الملف. |
| [hashCode()](#hashCode--) |  |
| [isExportComments()](#isExportComments--) | يحدد ما إذا كان يتم تصدير التعليقات عند حفظ الملف إلى HTML، القيمة الافتراضية هي false. |
| [isFullPathLink()](#isFullPathLink--) | الإشارة إلى ما إذا كان يتم استخدام رابط المسار الكامل في sheet00x.htm و filelist.xml و tabstrip.htm. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAttachedFilesDirectory(String value)](#setAttachedFilesDirectory-java.lang.String-) | الدليل الذي سيتم حفظ الملفات المرفقة فيه. |
| [setAttachedFilesUrlPrefix(String value)](#setAttachedFilesUrlPrefix-java.lang.String-) | حدد بادئة URL للملفات المرفقة مثل الصورة في ملف HTML. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | مجلد الملفات المؤقت يُستخدم لتخزين بعض البيانات الكبيرة. |
| [setClearData(boolean value)](#setClearData-boolean-) | اجعل دفتر العمل فارغًا بعد حفظ الملف. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | إذا كان صحيحًا ولم يكن الدليل موجودًا، فسيتم إنشاء الدليل تلقائيًا قبل حفظ الملف. |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | حدد اسم الخط الافتراضي لتصدير HTML، سيتم استخدام الخط الافتراضي عندما لا يكون خط النمط موجودًا، إذا كانت هذه الخاصية فارغة (null)، سيستخدم Aspose.Cells خطًا عالميًا يملك نفس عائلة الخط الأصلي، القيمة الافتراضية هي null. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.gridweb.Encoding-) | إذا لم يتم تحديده، استخدم Encoding.UTF8 كنمط الترميز الافتراضي. |
| [setExportActiveWorksheetOnly(boolean value)](#setExportActiveWorksheetOnly-boolean-) | يشير إلى ما إذا كان يتم تصدير المصنف بالكامل إلى ملف html. |
| [setExportArea(GridCellArea value)](#setExportArea-com.aspose.gridweb.GridCellArea-) | يضبط نطاق CellArea المُصدّر للورقة النشطة الحالية. |
| [setExportComments(boolean value)](#setExportComments-boolean-) | يحدد ما إذا كان يتم تصدير التعليقات عند حفظ الملف إلى HTML، القيمة الافتراضية هي false. |
| [setExportGridLines(boolean value)](#setExportGridLines-boolean-) | الإشارة إلى ما إذا كان يتم تصدير خطوط الشبكة. القيمة الافتراضية هي false. |
| [setExportHeadings(boolean value)](#setExportHeadings-boolean-) | يشير إلى ما إذا كان يتم تصدير العناوين عند حفظ الملف إلى html. القيمة الافتراضية هي false. |
| [setExportHiddenWorksheet(boolean value)](#setExportHiddenWorksheet-boolean-) | الإشارة إلى ما إذا كان يتم تصدير محتوى ورقة العمل المخفي. القيمة الافتراضية هي true. |
| [setExportImagesAsBase64(boolean value)](#setExportImagesAsBase64-boolean-) | يحدد ما إذا كانت الصور تُحفظ بتنسيق Base64 إلى HTML أو MHTML أو EPUB. |
| [setExportPrintAreaOnly(boolean value)](#setExportPrintAreaOnly-boolean-) | يحدد ما إذا كان يتم تصدير منطقة الطباعة فقط إلى ملف HTML. |
| [setExportSingleTab(boolean value)](#setExportSingleTab-boolean-) | يحدد ما إذا كان يتم تصدير علامة التبويب الوحيدة عندما يحتوي الملف على ورقة عمل واحدة فقط. |
| [setFullPathLink(boolean value)](#setFullPathLink-boolean-) | الإشارة إلى ما إذا كان يتم استخدام رابط المسار الكامل في sheet00x.htm و filelist.xml و tabstrip.htm. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | يحدد ما إذا كان يتم دمج مناطق التنسيق الشرطي والتحقق قبل حفظ الملف. |
| [setPageTitle(String value)](#setPageTitle-java.lang.String-) | عنوان صفحة HTML. |
|  | [setParseHtmlTagInCell(boolean value)](#setParseHtmlTagInCell-boolean-) | تحليل علامة html في الخلية، مثل |

، كقيمة خلية، أو كعلامة html، القيمة الافتراضية هي true |
| [setPresentationPreference(boolean value)](#setPresentationPreference-boolean-) | الإشارة إلى ما إذا كان ملف html أو mht هو تفضيل العرض. القيمة الافتراضية هي false. إذا كنت تريد الحصول على عرض أكثر جمالًا، يرجى ضبط القيمة إلى true. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | يشير إلى ما إذا كان يتم تحديث بيانات مخزن مؤقت المخطط |
| [setSortNames(boolean value)](#setSortNames-boolean-) | يحدد ما إذا كان يتم فرز الأسماء المعرفة قبل حفظ الملف. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | يحدد ما إذا كان يتم التحقق من صحة الخلايا المدمجة قبل حفظ الملف. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridHtmlSaveOptions() {#GridHtmlSaveOptions--}
```
public GridHtmlSaveOptions()
```


ينشئ خيارات لحفظ ملف html.

### GridHtmlSaveOptions(int format) {#GridHtmlSaveOptions-int-}
```
public GridHtmlSaveOptions(int format)
```


ينشئ خيارات لحفظ ملف htm.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| format | int | [GridSaveFormat](../../com.aspose.gridweb/gridsaveformat). تنسيق حفظ الملف. |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAttachedFilesDirectory() {#getAttachedFilesDirectory--}
```
public String getAttachedFilesDirectory()
```


الدليل الذي سيتم حفظ الملفات المرفقة فيه. يُستخدم فقط لحفظ تدفق HTML.

**Returns:**
java.lang.String
### getAttachedFilesUrlPrefix() {#getAttachedFilesUrlPrefix--}
```
public String getAttachedFilesUrlPrefix()
```


حدد بادئة URL للملفات المرفقة مثل الصورة في ملف HTML. يُستخدم فقط لحفظ تدفق HTML.

**Returns:**
java.lang.String
### getCachedFileFolder() {#getCachedFileFolder--}
```
public String getCachedFileFolder()
```


مجلد الملفات المؤقت يُستخدم لتخزين بعض البيانات الكبيرة.

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getClearData() {#getClearData--}
```
public boolean getClearData()
```


اجعل دفتر العمل فارغًا بعد حفظ الملف.

**Returns:**
boolean
### getCreateDirectory() {#getCreateDirectory--}
```
public boolean getCreateDirectory()
```


إذا كان صحيحًا ولم يكن الدليل موجودًا، فسيتم إنشاء الدليل تلقائيًا قبل حفظ الملف.

**Remarks**

القيمة الافتراضية هي false.

**Returns:**
boolean
### getDefaultFontName() {#getDefaultFontName--}
```
public String getDefaultFontName()
```


حدد اسم الخط الافتراضي لتصدير HTML، سيتم استخدام الخط الافتراضي عندما لا يكون خط النمط موجودًا، إذا كانت هذه الخاصية فارغة (null)، سيستخدم Aspose.Cells خطًا عالميًا يملك نفس عائلة الخط الأصلي، القيمة الافتراضية هي null.

**Returns:**
java.lang.String
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


إذا لم يتم تحديده، استخدم Encoding.UTF8 كنمط الترميز الافتراضي.

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding)
### getExportActiveWorksheetOnly() {#getExportActiveWorksheetOnly--}
```
public boolean getExportActiveWorksheetOnly()
```


يشير إلى ما إذا كان يتم تصدير المصنف بالكامل إلى ملف html.

**Returns:**
boolean
### getExportArea() {#getExportArea--}
```
public GridCellArea getExportArea()
```


يحصل على نطاق الخلية (CellArea) المُصدَّر للورقة النشطة الحالية. إذا قمت بتعيين هذه الخاصية، سيتم إهمال منطقة الطباعة للورقة النشطة الحالية. سيتم تصدير النطاق المحدد فقط عند حفظ الملف إلى html.

**Returns:**
[GridCellArea](../../com.aspose.gridweb/gridcellarea)
### getExportGridLines() {#getExportGridLines--}
```
public boolean getExportGridLines()
```


الإشارة إلى ما إذا كان يتم تصدير خطوط الشبكة. القيمة الافتراضية هي false.

**Returns:**
boolean
### getExportHeadings() {#getExportHeadings--}
```
public boolean getExportHeadings()
```


يشير إلى ما إذا كان يتم تصدير العناوين عند حفظ الملف إلى html. القيمة الافتراضية هي false. إذا كنت تريد استيراد ملف html إلى excel، يرجى الحفاظ على القيمة الافتراضية.

**Returns:**
boolean
### getExportHiddenWorksheet() {#getExportHiddenWorksheet--}
```
public boolean getExportHiddenWorksheet()
```


الإشارة إلى ما إذا كان يتم تصدير محتوى ورقة العمل المخفي. القيمة الافتراضية هي true.

**Returns:**
boolean
### getExportImagesAsBase64() {#getExportImagesAsBase64--}
```
public boolean getExportImagesAsBase64()
```


يحدد ما إذا كانت الصور تُحفظ بتنسيق Base64 إلى HTML أو MHTML أو EPUB.

**Remarks**

عند ضبط هذه الخاصية على true يتم تصدير بيانات الصورة مباشرةً على عناصر img ولا يتم إنشاء ملفات منفصلة.

**Returns:**
boolean
### getExportPrintAreaOnly() {#getExportPrintAreaOnly--}
```
public boolean getExportPrintAreaOnly()
```


يشير إلى ما إذا كان يتم تصدير منطقة الطباعة فقط إلى ملف html. القيمة الافتراضية هي false.

**Returns:**
boolean
### getExportSingleTab() {#getExportSingleTab--}
```
public boolean getExportSingleTab()
```


يشير إلى ما إذا كان يتم تصدير علامة التبويب الوحيدة عندما يحتوي الملف على ورقة عمل واحدة فقط. القيمة الافتراضية هي false.

**Returns:**
boolean
### getMergeAreas() {#getMergeAreas--}
```
public boolean getMergeAreas()
```


يحدد ما إذا كان يتم دمج مناطق التنسيق الشرطي والتحقق قبل حفظ الملف.

**Remarks**

القيمة الافتراضية هي false.

**Returns:**
boolean
### getPageTitle() {#getPageTitle--}
```
public String getPageTitle()
```


عنوان صفحة html. يستخدم فقط عند حفظ إلى تدفق html.

**Returns:**
java.lang.String
### getParseHtmlTagInCell() {#getParseHtmlTagInCell--}
```
public boolean getParseHtmlTagInCell()
```


تحليل علامة html في الخلية، مثل

، كقيمة خلية، أو كعلامة html، القيمة الافتراضية هي true

**Returns:**
boolean
### getPresentationPreference() {#getPresentationPreference--}
```
public boolean getPresentationPreference()
```


الإشارة إلى ما إذا كان ملف html أو mht هو تفضيل العرض. القيمة الافتراضية هي false. إذا كنت تريد الحصول على عرض أكثر جمالًا، يرجى ضبط القيمة إلى true.

**Returns:**
boolean
### getRefreshChartCache() {#getRefreshChartCache--}
```
public boolean getRefreshChartCache()
```


يشير إلى ما إذا كان يتم تحديث بيانات مخزن مؤقت المخطط

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


يحصل على صيغة حفظ الملف.

انظر [GridSaveFormat](../../com.aspose.gridweb/gridsaveformat).

**Returns:**
int
### getSortNames() {#getSortNames--}
```
public boolean getSortNames()
```


يحدد ما إذا كان يتم فرز الأسماء المعرفة قبل حفظ الملف.

**Returns:**
boolean
### getValidateMergedAreas() {#getValidateMergedAreas--}
```
public boolean getValidateMergedAreas()
```


يحدد ما إذا كان يتم التحقق من صحة الخلايا المدمجة قبل حفظ الملف.

**Remarks**

القيمة الافتراضية هي false.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isExportComments() {#isExportComments--}
```
public boolean isExportComments()
```


يحدد ما إذا كان يتم تصدير التعليقات عند حفظ الملف إلى HTML، القيمة الافتراضية هي false.

**Returns:**
boolean
### isFullPathLink() {#isFullPathLink--}
```
public boolean isFullPathLink()
```


تشير إلى ما إذا كان سيتم استخدام رابط المسار الكامل في sheet00x.htm, filelist.xml و tabstrip.htm. القيمة الافتراضية هي false.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAttachedFilesDirectory(String value) {#setAttachedFilesDirectory-java.lang.String-}
```
public void setAttachedFilesDirectory(String value)
```


الدليل الذي سيتم حفظ الملفات المرفقة فيه. يُستخدم فقط لحفظ تدفق HTML.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setAttachedFilesUrlPrefix(String value) {#setAttachedFilesUrlPrefix-java.lang.String-}
```
public void setAttachedFilesUrlPrefix(String value)
```


حدد بادئة URL للملفات المرفقة مثل الصورة في ملف HTML. يُستخدم فقط لحفظ تدفق HTML.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setCachedFileFolder(String value) {#setCachedFileFolder-java.lang.String-}
```
public void setCachedFileFolder(String value)
```


مجلد الملفات المؤقت يُستخدم لتخزين بعض البيانات الكبيرة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setClearData(boolean value) {#setClearData-boolean-}
```
public void setClearData(boolean value)
```


اجعل دفتر العمل فارغًا بعد حفظ الملف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setCreateDirectory(boolean value) {#setCreateDirectory-boolean-}
```
public void setCreateDirectory(boolean value)
```


إذا كان صحيحًا ولم يكن الدليل موجودًا، فسيتم إنشاء الدليل تلقائيًا قبل حفظ الملف.

**Remarks**

القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public void setDefaultFontName(String value)
```


حدد اسم الخط الافتراضي لتصدير HTML، سيتم استخدام الخط الافتراضي عندما لا يكون خط النمط موجودًا، إذا كانت هذه الخاصية فارغة (null)، سيستخدم Aspose.Cells خطًا عالميًا يملك نفس عائلة الخط الأصلي، القيمة الافتراضية هي null.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setEncoding(Encoding value) {#setEncoding-com.aspose.gridweb.Encoding-}
```
public void setEncoding(Encoding value)
```


إذا لم يتم تحديده، استخدم Encoding.UTF8 كنمط الترميز الافتراضي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.gridweb/encoding) |  |

### setExportActiveWorksheetOnly(boolean value) {#setExportActiveWorksheetOnly-boolean-}
```
public void setExportActiveWorksheetOnly(boolean value)
```


يشير إلى ما إذا كان يتم تصدير المصنف بالكامل إلى ملف html.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setExportArea(GridCellArea value) {#setExportArea-com.aspose.gridweb.GridCellArea-}
```
public void setExportArea(GridCellArea value)
```


يضبط نطاق الخلية (CellArea) المُصدَّر للورقة النشطة الحالية. إذا قمت بتعيين هذه الخاصية، سيتم إهمال منطقة الطباعة للورقة النشطة الحالية. سيتم تصدير النطاق المحدد فقط عند حفظ الملف إلى html.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [GridCellArea](../../com.aspose.gridweb/gridcellarea) |  |

### setExportComments(boolean value) {#setExportComments-boolean-}
```
public void setExportComments(boolean value)
```


يحدد ما إذا كان يتم تصدير التعليقات عند حفظ الملف إلى HTML، القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setExportGridLines(boolean value) {#setExportGridLines-boolean-}
```
public void setExportGridLines(boolean value)
```


الإشارة إلى ما إذا كان يتم تصدير خطوط الشبكة. القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setExportHeadings(boolean value) {#setExportHeadings-boolean-}
```
public void setExportHeadings(boolean value)
```


يشير إلى ما إذا كان يتم تصدير العناوين عند حفظ الملف إلى html. القيمة الافتراضية هي false. إذا كنت تريد استيراد ملف html إلى excel، يرجى الحفاظ على القيمة الافتراضية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setExportHiddenWorksheet(boolean value) {#setExportHiddenWorksheet-boolean-}
```
public void setExportHiddenWorksheet(boolean value)
```


الإشارة إلى ما إذا كان يتم تصدير محتوى ورقة العمل المخفي. القيمة الافتراضية هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setExportImagesAsBase64(boolean value) {#setExportImagesAsBase64-boolean-}
```
public void setExportImagesAsBase64(boolean value)
```


يحدد ما إذا كانت الصور تُحفظ بتنسيق Base64 إلى HTML أو MHTML أو EPUB.

**Remarks**

عند ضبط هذه الخاصية على true يتم تصدير بيانات الصورة مباشرةً على عناصر img ولا يتم إنشاء ملفات منفصلة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setExportPrintAreaOnly(boolean value) {#setExportPrintAreaOnly-boolean-}
```
public void setExportPrintAreaOnly(boolean value)
```


يشير إلى ما إذا كان يتم تصدير منطقة الطباعة فقط إلى ملف html. القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setExportSingleTab(boolean value) {#setExportSingleTab-boolean-}
```
public void setExportSingleTab(boolean value)
```


يشير إلى ما إذا كان يتم تصدير علامة التبويب الوحيدة عندما يحتوي الملف على ورقة عمل واحدة فقط. القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setFullPathLink(boolean value) {#setFullPathLink-boolean-}
```
public void setFullPathLink(boolean value)
```


تشير إلى ما إذا كان سيتم استخدام رابط المسار الكامل في sheet00x.htm, filelist.xml و tabstrip.htm. القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setMergeAreas(boolean value) {#setMergeAreas-boolean-}
```
public void setMergeAreas(boolean value)
```


يحدد ما إذا كان يتم دمج مناطق التنسيق الشرطي والتحقق قبل حفظ الملف.

**Remarks**

القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setPageTitle(String value) {#setPageTitle-java.lang.String-}
```
public void setPageTitle(String value)
```


عنوان صفحة html. يستخدم فقط عند حفظ إلى تدفق html.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setParseHtmlTagInCell(boolean value) {#setParseHtmlTagInCell-boolean-}
```
public void setParseHtmlTagInCell(boolean value)
```


تحليل علامة html في الخلية، مثل

، كقيمة خلية، أو كعلامة html، القيمة الافتراضية هي true

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setPresentationPreference(boolean value) {#setPresentationPreference-boolean-}
```
public void setPresentationPreference(boolean value)
```


الإشارة إلى ما إذا كان ملف html أو mht هو تفضيل العرض. القيمة الافتراضية هي false. إذا كنت تريد الحصول على عرض أكثر جمالًا، يرجى ضبط القيمة إلى true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


يشير إلى ما إذا كان يتم تحديث بيانات مخزن مؤقت المخطط

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setSortNames(boolean value) {#setSortNames-boolean-}
```
public void setSortNames(boolean value)
```


يحدد ما إذا كان يتم فرز الأسماء المعرفة قبل حفظ الملف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setValidateMergedAreas(boolean value) {#setValidateMergedAreas-boolean-}
```
public void setValidateMergedAreas(boolean value)
```


يحدد ما إذا كان يتم التحقق من صحة الخلايا المدمجة قبل حفظ الملف.

**Remarks**

القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

