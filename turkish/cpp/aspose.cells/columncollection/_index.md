---
title: Aspose::Cells::ColumnCollection class
linktitle: ColumnCollection
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::ColumnCollection class. Collection of the Column objects that represent the individual column(setting)s in a worksheet. The Column object only represents the settings such as column width, styles, .etc. for the whole column, has nothing to do with the fact that there are non-empty cells(data) or not in corresponding column. And the "Count" of this collection only represents the count Column objects that have been instantiated in this collection, has nothing to do with the fact that there are non-empty cells(data) or not in the worksheet in C++.'
type: docs
weight: 2800
url: /tr/cpp/aspose.cells/columncollection/
---
## ColumnCollection class


Collection of the [Column](../column/) objects that represent the individual column(setting)s in a worksheet. The [Column](../column/) object only represents the settings such as column width, styles, .etc. for the whole column, has nothing to do with the fact that there are non-empty cells(data) or not in corresponding column. And the "Count" of this collection only represents the count [Column](../column/) objects that have been instantiated in this collection, has nothing to do with the fact that there are non-empty cells(data) or not in the worksheet.

```cpp
class ColumnCollection
```

## Methods

| Method | Description |
| --- | --- |
| [begin()](./begin/) | Returns an iterator to the beginning of the [ColumnCollection](./). |
| [ColumnCollection(ColumnCollection_Impl* impl)](./columncollection/) | Constructs from an implementation object. |
| [ColumnCollection(const ColumnCollection\& src)](./columncollection/) | Copy constructor. |
| [end()](./end/) | Returns an iterator to the end of the [ColumnCollection](./). |
| [Get(int32_t columnIndex)](./get/) | Gets a [Column](../column/) object by column index. The [Column](../column/) object of given column index will be instantiated if it does not exist before. |
| [GetColumnByIndex(int32_t index)](./getcolumnbyindex/) | Gets the [Column](../column/) object by the position in the list. |
| [GetCount()](./getcount/) | Gets the number of elements contained in the instance. |
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
//Bir Workbook nesnesi oluşturuluyor
Workbook workbook;

//İlk çalışma sayfasının referansını elde etme
Worksheet worksheet = workbook.GetWorksheets().Get(0);

//Çalışma Kitabına yeni Stil ekle
Style style = workbook.CreateStyle();

//Arka plan rengini Mavi olarak ayarlama
style.SetForegroundColor(Color{ 0xff, 0, 0, 0xff });

//Arka plan desenini ayarlama
style.SetPattern(BackgroundType::Solid);

//Yeni Stil Bayrağı
StyleFlag styleFlag;

//Tüm Stilleri Ayarla
styleFlag.SetAll(true);

//İlk on sütunun varsayılan genişliğini değiştir
for (int i = 0; i < 10; i++)
{
    worksheet.GetCells().GetColumns().Get(i).SetWidth(20);
}

//Varsayılan olmayan biçimlendirmeye sahip sütunu al
ColumnCollection columns = worksheet.GetCells().GetColumns();

for (int i = 0; i < columns.GetCount(); ++i)
{
    Column column = columns.Get(i);
    //İlk on sütuna Stil uygula
    column.ApplyStyle(style, styleFlag);
}

//Excel dosyasını kaydetme
workbook.Save(u"book1.xls");

Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
