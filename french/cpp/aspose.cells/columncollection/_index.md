---
title: Aspose::Cells::ColumnCollection class
linktitle: ColumnCollection
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::ColumnCollection class. Collection of the Column objects that represent the individual column(setting)s in a worksheet. The Column object only represents the settings such as column width, styles, .etc. for the whole column, has nothing to do with the fact that there are non-empty cells(data) or not in corresponding column. And the "Count" of this collection only represents the count Column objects that have been instantiated in this collection, has nothing to do with the fact that there are non-empty cells(data) or not in the worksheet in C++.'
type: docs
weight: 2800
url: /fr/cpp/aspose.cells/columncollection/
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
//Instanciation d'un objet Workbook
Workbook workbook;

//Obtention de la référence de la première feuille de calcul
Worksheet worksheet = workbook.GetWorksheets().Get(0);

//Ajouter un nouveau style au classeur
Style style = workbook.CreateStyle();

//Définir la couleur d'arrière-plan sur Bleu
style.SetForegroundColor(Color{ 0xff, 0, 0, 0xff });

//définir le motif d'arrière-plan
style.SetPattern(BackgroundType::Solid);

//Nouveau drapeau de style
StyleFlag styleFlag;

//Définir tous les styles
styleFlag.SetAll(true);

//Modifier la largeur par défaut des dix premières colonnes
for (int i = 0; i < 10; i++)
{
    worksheet.GetCells().GetColumns().Get(i).SetWidth(20);
}

//Obtenir la colonne avec un formatage non par défaut
ColumnCollection columns = worksheet.GetCells().GetColumns();

for (int i = 0; i < columns.GetCount(); ++i)
{
    Column column = columns.Get(i);
    //Appliquer le style aux dix premières colonnes
    column.ApplyStyle(style, styleFlag);
}

//Enregistrement du fichier Excel
workbook.Save(u"book1.xls");

Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
