---
title: Aspose::Cells::ColumnCollection class
linktitle: ColumnCollection
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::ColumnCollection class. Collection of the Column objects that represent the individual column(setting)s in a worksheet. The Column object only represents the settings such as column width, styles, .etc. for the whole column, has nothing to do with the fact that there are non-empty cells(data) or not in corresponding column. And the "Count" of this collection only represents the count Column objects that have been instantiated in this collection, has nothing to do with the fact that there are non-empty cells(data) or not in the worksheet in C++.'
type: docs
weight: 2800
url: /de/cpp/aspose.cells/columncollection/
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
//Instanziieren eines Workbook-Objekts
Workbook workbook;

//Abrufen der Referenz des ersten Arbeitsblatts
Worksheet worksheet = workbook.GetWorksheets().Get(0);

//Neuen Stil zum Arbeitsbuch hinzufügen
Style style = workbook.CreateStyle();

//Hintergrundfarbe auf Blau setzen
style.SetForegroundColor(Color{ 0xff, 0, 0, 0xff });

//Hintergrundmuster festlegen
style.SetPattern(BackgroundType::Solid);

//Neues Stil-Flag
StyleFlag styleFlag;

//Alle Stile festlegen
styleFlag.SetAll(true);

//Ändern Sie die Standardbreite der ersten zehn Spalten
for (int i = 0; i < 10; i++)
{
    worksheet.GetCells().GetColumns().Get(i).SetWidth(20);
}

//Rufen Sie die Spalte mit nicht standardmäßiger Formatierung ab
ColumnCollection columns = worksheet.GetCells().GetColumns();

for (int i = 0; i < columns.GetCount(); ++i)
{
    Column column = columns.Get(i);
    //Stil auf die ersten zehn Spalten anwenden
    column.ApplyStyle(style, styleFlag);
}

//Speichern der Excel-Datei
workbook.Save(u"book1.xls");

Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
