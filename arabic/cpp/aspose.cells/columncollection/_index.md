---
title: Aspose::Cells::ColumnCollection class
linktitle: ColumnCollection
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::ColumnCollection class. Collection of the Column objects that represent the individual column(setting)s in a worksheet. The Column object only represents the settings such as column width, styles, .etc. for the whole column, has nothing to do with the fact that there are non-empty cells(data) or not in corresponding column. And the "Count" of this collection only represents the count Column objects that have been instantiated in this collection, has nothing to do with the fact that there are non-empty cells(data) or not in the worksheet in C++.'
type: docs
weight: 2800
url: /ar/cpp/aspose.cells/columncollection/
---
## ColumnCollection class


Collection of the [Column](../column/) objects that represent the individual column(setting)s in a worksheet. The [Column](../column/) object only represents the settings such as column width, styles, .etc. for the whole column, has nothing to do with the fact that there are non-empty cells(data) or not in corresponding column. And the "Count" of this collection only represents the count [Column](../column/) objects that have been instantiated in this collection, has nothing to do with the fact that there are non-empty cells(data) or not in the worksheet.

```cpp
class ColumnCollection
```

## Methods

| Method | Description |
| --- | --- |
| [ColumnCollection(ColumnCollection_Impl* impl)](./columncollection/) | Constructs from an implementation object. |
| [ColumnCollection(const ColumnCollection\& src)](./columncollection/) | Copy constructor. |
| [Get(int32_t columnIndex)](./get/) | Gets a [Column](../column/) object by column index. The [Column](../column/) object of given column index will be instantiated if it does not exist before. |
| [GetColumnByIndex(int32_t index)](./getcolumnbyindex/) | Gets the [Column](../column/) object by the position in the list. |
| [GetCount()](./getcount/) |  |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const ColumnCollection\& src)](./operator_asm/) | operator= |
| [~ColumnCollection()](./~columncollection/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |

## Examples


```cpp
Aspose::Cells::Startup();
//إنشاء كائن Workbook
Workbook workbook;

//الحصول على مرجع الورقة الأولى
Worksheet worksheet = workbook.GetWorksheets().Get(0);

//إضافة نمط جديد إلى المصنف
Style style = workbook.CreateStyle();

//Setting the background color to Blue
style.SetForegroundColor(Color{ 0xff, 0, 0, 0xff });

//setting Background Pattern
style.SetPattern(BackgroundType::Solid);

//New Style Flag
StyleFlag styleFlag;

//Set All Styles
styleFlag.SetAll(true);

//تغيير العرض الافتراضي للأعمدة العشرة الأولى
for (int i = 0; i < 10; i++)
{
    worksheet.GetCells().GetColumns().Get(i).SetWidth(20);
}

//الحصول على العمود بتنسيق غير افتراضي
ColumnCollection columns = worksheet.GetCells().GetColumns();

for (int i = 0; i < columns.GetCount(); ++i)
{
    Column column = columns.Get(i);
    //تطبيق النمط على الأعمدة العشرة الأولى
    column.ApplyStyle(style, styleFlag);
}

//حفظ ملف Excel
workbook.Save(u"book1.xls");

Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
