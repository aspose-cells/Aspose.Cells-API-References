---
title: PdfBookmarkEntry класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 80
url: /ru/python-net/aspose.cells.rendering/pdfbookmarkentry/
is_root: false
---
##  PdfBookmarkEntry класс
PdfBookmarkEntry — запись в закладке pdf.
если свойство Text текущего экземпляра равно null или "",
текущий экземпляр будет скрыт, а дочерние элементы будут вставлены на текущий уровень.



Тип PdfBookmarkEntry предоставляет следующие члены:

###  Конструкторы
| Конструктор| Описание|
| :- | :- |
| [PdfBookmarkEntry()](/cells/ru/python-net/aspose.cells.rendering/pdfbookmarkentry/__init__/#) | Создает новый экземпляр PdfBookmarkEntry|


###  Характеристики
| Свойство| Описание|
| :- | :- |
| [text](/cells/ru/python-net/aspose.cells.rendering/pdfbookmarkentry/text) | Название закладки.|
| [destination](/cells/ru/python-net/aspose.cells.rendering/pdfbookmarkentry/destination) | Ячейка, на которую ссылается закладка.|
| [destination_name](/cells/ru/python-net/aspose.cells.rendering/pdfbookmarkentry/destination_name) | Получает или задает имя места назначения.|
| [sub_entry](/cells/ru/python-net/aspose.cells.rendering/pdfbookmarkentry/sub_entry) | SubEntry закладки.|
| [is_open](/cells/ru/python-net/aspose.cells.rendering/pdfbookmarkentry/is_open) |Когда это свойство имеет значение true, запись закладки будет расширяться, в противном случае она свернется.|
| [is_collapse](/cells/ru/python-net/aspose.cells.rendering/pdfbookmarkentry/is_collapse) | Когда это свойство имеет значение true, запись закладки свернется, в противном случае она расширится.|



###  Пример

```python
from aspose.cells import PdfSaveOptions, Workbook
from aspose.cells.rendering import PdfBookmarkEntry

workbook = Workbook()
workbook.worksheets.add()
workbook.worksheets.add()
cellInPage1 = workbook.worksheets[0].cells.get("A1")
cellInPage2 = workbook.worksheets[1].cells.get("A1")
cellInPage3 = workbook.worksheets[2].cells.get("A1")
cellInPage1.put_value("page1")
cellInPage2.put_value("page2")
cellInPage3.put_value("page3")
pbeRoot = PdfBookmarkEntry()
pbeRoot.text = "root"
pbeRoot.destination = cellInPage1
pbeRoot.sub_entry = []
pbeRoot.is_open = False
subPbe1 = PdfBookmarkEntry()
subPbe1.text = "section1"
subPbe1.destination = cellInPage2
subPbe2 = PdfBookmarkEntry()
subPbe2.text = "section2"
subPbe2.destination = cellInPage3
pbeRoot.sub_entry.append(subPbe1)
pbeRoot.sub_entry.append(subPbe2)
saveOptions = PdfSaveOptions()
saveOptions.bookmark = pbeRoot
workbook.save("output_bookmark.pdf", saveOptions)

```

###  Смотрите также
* модуль [aspose.cells.rendering](..)
