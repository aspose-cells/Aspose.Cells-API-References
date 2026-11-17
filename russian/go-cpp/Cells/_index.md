---
title: "Класс Cells"
linktitle: "Cells"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс Cells. Инкапсулирует объект, представляющий ячейки в Go."
type: docs
weight: 200
url: /ru/go-cpp/cells/
---

## Cells class

Инкапсулирует коллекцию объектов, связанных с ячейкой, таких как <see cref=\"Cell\"/>, <see cref=\"Row\"/> и т.д.

```go

type Cells struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetOdsCellFields](./getodscellfields/) | Получает список полей ods. |
| [Dispose](./dispose/) | Выполняет задачи, определённые приложением, связанные с освобождением, выпуском или сбросом неуправляемых ресурсов. |
| [GetCount](./getcount/) | Получает общее количество созданных объектов Cell. |
| [GetCountLarge](./getcountlarge/) | Получает общее количество созданных объектов Cell. |
| [GetEnumerator](./getenumerator/) | Получает перечислитель ячеек. |
| [GetRows](./getrows/) | Получает коллекцию объектов Row, представляющих отдельные строки в этом листе. |
| [GetMergedAreas](./getmergedareas/) | Получает все объединённые ячейки. |
| [CheckCell](./checkcell/) | Получает элемент Cell или null по указанному индексу строки ячейки и индексу столбца. |
| [CheckRow](./checkrow/) | Получает элемент Row или null по указанному индексу строки ячейки. |
| [CheckColumn](./checkcolumn/) | Получает элемент Column или null по указанному индексу столбца. |
| [IsRowHidden](./isrowhidden/) | Проверяет, скрыта ли строка с заданным индексом. |
| [IsColumnHidden](./iscolumnhidden/) | Проверяет, скрыт ли столбец с заданным индексом. |
| [AddRange](./addrange/) | Добавляет ссылку на объект диапазона к ячейкам |
| [CreateRange_String_String](./createrange_string_string/) | Создает объект Range из диапазона ячеек. |
| [CreateRange_Int_Int_Int_Int](./createrange_int_int_int_int/) | Создает объект Range из диапазона ячеек. |
| [CreateRange_String](./createrange_string/) | Создает объект Range из адреса диапазона. |
| [CreateRange_Int_Int_Bool](./createrange_int_int_bool/) | Создает объект Range из строк ячеек или столбцов ячеек. |
| [Get_Int_Int](./get_int_int/) | Получает элемент Cell по указанному индексу строки ячейки и индексу столбца. |
| [Get_String](./get_string/) | Получает элемент Cell по указанному имени ячейки. |
| [GetMultiThreadReading](./getmultithreadreading/) | Получает или задает, должна ли модель данных ячеек поддерживать многопоточное чтение. Значение свойства по умолчанию — false. |
| [SetMultiThreadReading](./setmultithreadreading/) | Получает или задает, должна ли модель данных ячеек поддерживать многопоточное чтение. Значение свойства по умолчанию — false. |
| [GetMemorySetting](./getmemorysetting/) | Получает или задает параметр использования памяти для этих ячеек. |
| [SetMemorySetting](./setmemorysetting/) | Получает или задает параметр использования памяти для этих ячеек. |
| [Clear](./clear/) | Очищает все данные листа. |
| [GetStyle](./getstyle/) | Получает и задает стиль по умолчанию листа. |
| [SetStyle](./setstyle/) | Получает и задает стиль по умолчанию листа. |
|[IsDefaultColumnHidden](./isdefaultcolumnhidden/) |  | 
|[SetIsDefaultColumnHidden](./setisdefaultcolumnhidden/) |  | 
| [GetStandardWidthInch](./getstandardwidthinch/) | Получает или задает ширину столбца по умолчанию в листе, в дюймах. |
| [SetStandardWidthInch](./setstandardwidthinch/) | Получает или задает ширину столбца по умолчанию в листе, в дюймах. |
| [GetStandardWidthPixels](./getstandardwidthpixels/) | Получает или задает ширину столбца по умолчанию в листе, в пикселях. |
| [SetStandardWidthPixels](./setstandardwidthpixels/) | Получает или задает ширину столбца по умолчанию в листе, в пикселях. |
| [GetStandardWidth](./getstandardwidth/) | Получает или задает ширину столбца по умолчанию в листе, в символах. |
| [SetStandardWidth](./setstandardwidth/) | Получает или задает ширину столбца по умолчанию в листе, в символах. |
| [GetStandardHeight](./getstandardheight/) | Получает или задает высоту строки по умолчанию в этом листе, в пунктах. |
| [SetStandardHeight](./setstandardheight/) | Получает или задает высоту строки по умолчанию в этом листе, в пунктах. |
| [GetStandardHeightPixels](./getstandardheightpixels/) | Получает или задает высоту строки по умолчанию в этом листе, в пикселях. |
| [SetStandardHeightPixels](./setstandardheightpixels/) | Получает или задает высоту строки по умолчанию в этом листе, в пикселях. |
| [GetStandardHeightInch](./getstandardheightinch/) | Получает или задает высоту строки по умолчанию в этом листе, в дюймах. |
| [SetStandardHeightInch](./setstandardheightinch/) | Получает или задает высоту строки по умолчанию в этом листе, в дюймах. |
| [ImportFormulaArray](./importformulaarray/) | Импортирует массив формул в лист. |
| [TextToColumns](./texttocolumns/) | Разделяет содержимое указанного столбца на несколько столбцов. |
| [ImportCSV_String_String_Bool_Int_Int](./importcsv_string_string_bool_int_int/) | Импортирует CSV‑файл в ячейки. |
| [ImportCSV_Stream_String_Bool_Int_Int](./importcsv_stream_string_bool_int_int/) | Импортирует CSV‑файл в ячейки. |
| [ImportCSV_String_TxtLoadOptions_Int_Int](./importcsv_string_txtloadoptions_int_int/) | Импортирует CSV‑файл в ячейки. |
| [ImportCSV_Stream_TxtLoadOptions_Int_Int](./importcsv_stream_txtloadoptions_int_int/) | Импортирует CSV‑файл в ячейки. |
| [GetPreserveString](./getpreservestring/) | Получает или задает значение, указывающее, сохраняются ли все значения листа как строки. По умолчанию — false. |
| [SetPreserveString](./setpreservestring/) | Получает или задает значение, указывающее, сохраняются ли все значения листа как строки. По умолчанию — false. |
| [Merge_Int_Int_Int_Int](./merge_int_int_int_int/) | Объединяет указанный диапазон ячеек в одну ячейку. |
| [Merge_Int_Int_Int_Int_Bool](./merge_int_int_int_int_bool/) | Объединяет указанный диапазон ячеек в одну ячейку. |
| [Merge_Int_Int_Int_Int_Bool_Bool](./merge_int_int_int_int_bool_bool/) | Объединяет указанный диапазон ячеек в одну ячейку. |
| [UnMerge](./unmerge/) | Разъединяет указанный диапазон объединённых ячеек. |
| [ClearMergedCells](./clearmergedcells/) | Очищает все объединённые диапазоны. |
| [HideRow](./hiderow/) | Скрывает строку. |
| [UnhideRow](./unhiderow/) | Отображает строку. |
| [HideRows](./hiderows/) | Скрывает несколько строк. |
| [UnhideRows](./unhiderows/) | Отображает скрытые строки. |
| [SetRowHeightPixel](./setrowheightpixel/) | Устанавливает высоту строки в пикселях. |
| [SetRowHeightInch](./setrowheightinch/) | Устанавливает высоту строки в дюймах. |
| [SetRowHeight](./setrowheight/) | Устанавливает высоту указанной строки. |
| [GetRowHeight_Int_Bool_CellsUnitType](./getrowheight_int_bool_cellsunittype/) | Получает высоту строки. |
| [GetColumnWidth_Int_Bool_CellsUnitType](./getcolumnwidth_int_bool_cellsunittype/) | Получает ширину столбца. |
| [HideColumn](./hidecolumn/) | Скрывает столбец. |
| [UnhideColumn](./unhidecolumn/) | Отображает столбец |
| [HideColumns](./hidecolumns/) | Скрывает несколько столбцов. |
| [UnhideColumns](./unhidecolumns/) | Отображает несколько столбцов. |
| [GetRowHeight_Int](./getrowheight_int/) | Получает высоту указанной строки в пунктах. |
| [GetViewRowHeight](./getviewrowheight/) | Получает высоту указанной строки. |
| [GetRowHeightInch](./getrowheightinch/) | Получает высоту указанной строки в дюймах. |
| [GetViewRowHeightInch](./getviewrowheightinch/) | Получает высоту указанной строки в дюймах. |
| [GetRowHeightPixel](./getrowheightpixel/) | Получает высоту указанной строки в пикселях. |
| [SetColumnWidthPixel](./setcolumnwidthpixel/) | Устанавливает ширину столбца в пикселях в обычном виде. |
| [SetColumnWidthInch](./setcolumnwidthinch/) | Устанавливает ширину столбца в дюймах в обычном виде. |
| [SetColumnWidth](./setcolumnwidth/) | Устанавливает ширину указанного столбца в обычном виде. |
| [GetColumnWidthPixel](./getcolumnwidthpixel/) | Получает ширину указанного столбца в обычном виде в пикселях. |
| [GetColumnWidth_Int](./getcolumnwidth_int/) | Получает ширину (в символах) указанного столбца в обычном виде |
| [GetViewColumnWidthPixel](./getviewcolumnwidthpixel/) | Получить ширину в разных типах представления. |
| [SetViewColumnWidthPixel](./setviewcolumnwidthpixel/) | Устанавливает ширину столбца в разных представлениях. |
| [GetMinRow](./getminrow/) | Минимальный индекс строки ячейки, содержащей данные или стиль. |
| [GetMaxRow](./getmaxrow/) | Максимальный индекс строки ячейки, содержащей данные или стиль. |
| [GetMinColumn](./getmincolumn/) | Минимальный индекс столбца тех ячеек, которые были созданы в коллекции (не включает столбец, для которого стиль определён для всего столбца, но ни одна ячейка не была создана). |
| [GetMaxColumn](./getmaxcolumn/) | Максимальный индекс столбца тех ячеек, которые были созданы в коллекции (не включает столбец, для которого стиль определён для всего столбца, но ни одна ячейка в нём не была создана). |
| [GetMinDataRow](./getmindatarow/) | Минимальный индекс строки ячейки, содержащей данные. |
| [GetMaxDataRow](./getmaxdatarow/) | Максимальный индекс строки ячейки, содержащей данные. |
| [GetMinDataColumn](./getmindatacolumn/) | Минимальный индекс столбца ячейки, содержащей данные. |
| [GetMaxDataColumn](./getmaxdatacolumn/) | Максимальный индекс столбца ячейки, содержащей данные. |
| [GetLastDataRow](./getlastdatarow/) | Получает последний индекс строки ячейки, содержащей данные в указанном столбце. |
| [GetFirstDataRow](./getfirstdatarow/) | Получает первый индекс строки ячейки, содержащей данные в указанном столбце. |
| [IsDefaultRowHeightMatched](./isdefaultrowheightmatched/) | Указывает, что высота строки и высота шрифта по умолчанию совпадают |
| [SetIsDefaultRowHeightMatched](./setisdefaultrowheightmatched/) | Указывает, что высота строки и высота шрифта по умолчанию совпадают |
| [IsDefaultRowHidden](./isdefaultrowhidden/) | Указывает, скрыта ли строка по умолчанию. |
| [SetIsDefaultRowHidden](./setisdefaultrowhidden/) | Указывает, скрыта ли строка по умолчанию. |
| [GetColumns](./getcolumns/) | Получает коллекцию объектов Column, представляющих отдельные столбцы в этом листе. |
| [ApplyColumnStyle](./applycolumnstyle/) | Применяет форматы ко всему столбцу. |
| [ApplyRowStyle](./applyrowstyle/) | Применяет форматы ко всей строке. |
| [ApplyStyle](./applystyle/) | Применяет форматы ко всему листу. |
| [CopyColumns_Cells_Int_Int_Int_PasteOptions](./copycolumns_cells_int_int_int_pasteoptions/) | Копирует данные и форматы всего столбца. |
| [CopyColumn](./copycolumn/) | Копирует данные и форматы всего столбца. |
| [CopyColumns_Cells_Int_Int_Int](./copycolumns_cells_int_int_int/) | Копирует данные и форматы целых столбцов. |
| [CopyColumns_Cells_Int_Int_Int_Int](./copycolumns_cells_int_int_int_int/) | Копирует данные и форматы всех столбцов. |
| [CopyRow](./copyrow/) | Копирует данные и форматы всей строки. |
| [CopyRows_Cells_Int_Int_Int](./copyrows_cells_int_int_int/) | Копирует данные и форматы некоторых целых строк. |
| [CopyRows_Cells_Int_Int_Int_CopyOptions](./copyrows_cells_int_int_int_copyoptions/) | Копирует данные и форматы некоторых целых строк. |
| [CopyRows_Cells_Int_Int_Int_CopyOptions_PasteOptions](./copyrows_cells_int_int_int_copyoptions_pasteoptions/) | Копирует данные и форматы некоторых целых строк. |
| [GetGroupedRowOutlineLevel](./getgroupedrowoutlinelevel/) | Получает уровень структуры (ноль‑базовый) строки. |
| [GetGroupedColumnOutlineLevel](./getgroupedcolumnoutlinelevel/) | Получает уровень структуры (ноль‑базовый) столбца. |
| [GetMaxGroupedColumnOutlineLevel](./getmaxgroupedcolumnoutlinelevel/) | Получает максимальный уровень структуры сгруппированных столбцов (ноль‑базовый). |
| [GetMaxGroupedRowOutlineLevel](./getmaxgroupedrowoutlinelevel/) | Получает максимальный уровень структуры сгруппированных строк (ноль‑базовый). |
| [ShowGroupDetail](./showgroupdetail/) | Разворачивает сгруппированные строки/столбцы. |
| [HideGroupDetail](./hidegroupdetail/) | Сворачивает сгруппированные строки/столбцы. |
| [UngroupColumns](./ungroupcolumns/) | Разгруппирует столбцы. |
| [GroupColumns_Int_Int](./groupcolumns_int_int/) | Группирует столбцы. |
| [GroupColumns_Int_Int_Bool](./groupcolumns_int_int_bool/) | Группирует столбцы. |
| [UngroupRows_Int_Int_Bool](./ungrouprows_int_int_bool/) | Разгруппирует строки. |
| [UngroupRows_Int_Int](./ungrouprows_int_int/) | Разгруппирует строки. |
| [GroupRows_Int_Int_Bool](./grouprows_int_int_bool/) | Группирует строки. |
| [GroupRows_Int_Int](./grouprows_int_int/) | Группирует строки. |
| [DeleteColumn_Int_Bool](./deletecolumn_int_bool/) | Удаляет столбец. |
| [DeleteColumn_Int](./deletecolumn_int/) | Удаляет столбец. |
| [DeleteColumns_Int_Int_Bool](./deletecolumns_int_int_bool/) | Удаляет несколько столбцов. |
| [DeleteColumns_Int_Int_DeleteOptions](./deletecolumns_int_int_deleteoptions/) | Удаляет несколько столбцов. |
| [IsDeletingRangeEnabled](./isdeletingrangeenabled/) | Проверьте, может ли диапазон быть удалён. |
| [DeleteRow_Int](./deleterow_int/) | Удаляет строку. |
| [DeleteRow_Int_Bool](./deleterow_int_bool/) | Удаляет строку. |
| [DeleteRows_Int_Int](./deleterows_int_int/) | Удаляет несколько строк. |
| [DeleteRows_Int_Int_Bool](./deleterows_int_int_bool/) | Удаляет несколько строк в листе. |
| [DeleteRows_Int_Int_DeleteOptions](./deleterows_int_int_deleteoptions/) | Удаляет несколько строк в листе. |
| [DeleteBlankColumns](./deleteblankcolumns/) | Удалить все пустые столбцы, которые не содержат данных. |
| [DeleteBlankColumns_DeleteOptions](./deleteblankcolumns_deleteoptions/) | Удалить все пустые столбцы, которые не содержат данных. |
| [IsBlankColumn](./isblankcolumn/) | Проверяет, является ли указанный столбец пустым (не содержит данных). |
| [DeleteBlankRows](./deleteblankrows/) | Удалить все пустые строки, которые не содержат данных или других объектов. |
| [DeleteBlankRows_DeleteOptions](./deleteblankrows_deleteoptions/) | Удалить все пустые строки, которые не содержат данных или некоторых специальных объектов, таких как видимый комментарий, сводная таблица. |
| [InsertColumns_Int_Int](./insertcolumns_int_int/) | Вставляет несколько столбцов в лист. |
| [InsertColumns_Int_Int_Bool](./insertcolumns_int_int_bool/) | Вставляет несколько столбцов в лист. |
| [InsertColumns_Int_Int_InsertOptions](./insertcolumns_int_int_insertoptions/) | Вставляет несколько столбцов в лист. |
| [InsertColumn_Int_Bool](./insertcolumn_int_bool/) | Вставляет новый столбец в лист. |
| [InsertColumn_Int](./insertcolumn_int/) | Вставляет новый столбец в лист. |
| [InsertRows_Int_Int_Bool](./insertrows_int_int_bool/) | Вставляет несколько строк в лист. |
| [InsertRows_Int_Int_InsertOptions](./insertrows_int_int_insertoptions/) | Вставляет несколько строк в лист. |
| [InsertRows_Int_Int](./insertrows_int_int/) | Вставляет несколько строк в лист. |
| [InsertRow](./insertrow/) | Вставляет новую строку в лист. |
| [GetRanges](./getranges/) | Получает коллекцию объектов Range, созданных во время выполнения. |
| [ClearRange_CellArea](./clearrange_cellarea/) | Очищает содержимое и форматирование диапазона. |
| [ClearRange_Int_Int_Int_Int](./clearrange_int_int_int_int/) | Очищает содержимое и форматирование диапазона. |
| [ClearContents_CellArea](./clearcontents_cellarea/) | Очищает содержимое диапазона. |
| [ClearContents_Int_Int_Int_Int](./clearcontents_int_int_int_int/) | Очищает содержимое диапазона. |
| [ClearFormats_CellArea](./clearformats_cellarea/) | Очищает форматирование диапазона. |
| [ClearFormats_Int_Int_Int_Int](./clearformats_int_int_int_int/) | Очищает форматирование диапазона. |
| [GetLastCell](./getlastcell/) | Получает последнюю ячейку в этом листе. |
| [LinkToXmlMap](./linktoxmlmap/) | Ссылка на XML‑карту. |
| [GetMaxDisplayRange](./getmaxdisplayrange/) | Получает максимальный диапазон, включающий данные, объединённые ячейки и фигуры. |
| [GetFirstCell](./getfirstcell/) | Получает первую ячейку в этом листе. |
| [Find_Object_Cell](./find_object_cell/) | Находит ячейку, содержащую входной объект. |
| [Find_Object_Cell_FindOptions](./find_object_cell_findoptions/) | Находит ячейку, содержащую входной объект. |
| [EndCellInRow_Int](./endcellinrow_int/) | Получает последнюю ячейку в этой строке. |
| [EndCellInColumn_Int](./endcellincolumn_int/) | Получает последнюю ячейку в этом столбце. |
| [EndCellInColumn_Int_Int_Int_Int](./endcellincolumn_int_int_int_int/) | Получает последнюю ячейку с максимальным индексом столбца в этом диапазоне. |
| [EndCellInRow_Int_Int_Int_Int](./endcellinrow_int_int_int_int/) | Получает последнюю ячейку с максимальным индексом строки в этом диапазоне. |
| [MoveRange](./moverange/) | Перемещает диапазон. |
| [InsertCutCells](./insertcutcells/) | Вставить вырезанный диапазон. |
| [InsertRange_CellArea_Int_ShiftType_Bool](./insertrange_cellarea_int_shifttype_bool/) | Вставляет диапазон ячеек и сдвигает ячейки в соответствии с параметром сдвига. |
| [InsertRange_CellArea_ShiftType](./insertrange_cellarea_shifttype/) | Вставляет диапазон ячеек и сдвигает ячейки в соответствии с параметром сдвига. |
| [InsertRange_CellArea_Int_ShiftType](./insertrange_cellarea_int_shifttype/) | Вставляет диапазон ячеек и сдвигает ячейки в соответствии с параметром сдвига. |
| [DeleteRange](./deleterange/) | Удаляет диапазон ячеек и сдвигает ячейки в соответствии с параметром сдвига. |
| [ExportArray](./exportarray/) | Экспортирует данные из коллекции Cells в объект двумерного массива. |
| [RetrieveSubtotalSetting](./retrievesubtotalsetting/) | Получает настройки промежуточных итогов диапазона. |
| [Subtotal_CellArea_Int_ConsolidationFunction_int32Array](./subtotal_cellarea_int_consolidationfunction_int32array/) | Создает промежуточные итоги для диапазона. |
| [Subtotal_CellArea_Int_ConsolidationFunction_int32Array_Bool_Bool_Bool](./subtotal_cellarea_int_consolidationfunction_int32array_bool_bool_bool/) | Создает промежуточные итоги для диапазона. |
| [RemoveFormulas](./removeformulas/) | Удаляет все формулы и заменяет их значением формулы. |
| [RemoveDuplicates](./removeduplicates/) | Удаляет дублирующиеся строки на листе. |
| [RemoveDuplicates_Int_Int_Int_Int](./removeduplicates_int_int_int_int/) | Удаляет дублирующиеся значения в диапазоне. |
| [RemoveDuplicates_Int_Int_Int_Int_Bool_int32Array](./removeduplicates_int_int_int_int_bool_int32array/) | Удаляет дублирующиеся данные диапазона. |
| [ConvertStringToNumericValue](./convertstringtonumericvalue/) | Преобразует все строковые данные в листе в числовое значение, если это возможно. |
| [GetDependents](./getdependents/) | Получить все ячейки, которые ссылаются на конкретную ячейку. |
| [GetDependentsInCalculation](./getdependentsincalculation/) | Получает все ячейки, чей вычисленный результат зависит от конкретной ячейки. |
| [GetCellsWithPlaceInCellPicture](./getcellswithplaceincellpicture/) | Получает все ячейки, содержащие встроенное изображение. |
| [GetCellStyle](./getcellstyle/) | Получить стиль заданной ячейки. |
| [GetCellDisplayStyle_Int_Int](./getcelldisplaystyle_int_int/) | Получить отображаемый стиль заданной ячейки. |
| [GetCellDisplayStyle_Int_Int_BorderType](./getcelldisplaystyle_int_int_bordertype/) | Получить отображаемый стиль заданной ячейки. |
