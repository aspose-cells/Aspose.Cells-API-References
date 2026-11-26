---
title: "ExternalLinkCollection.Clear"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ExternalLinkCollection. Удаляет все внешние ссылки"
type: docs
url: /ru/net/aspose.cells/externallinkcollection/clear/
---
## Clear() {#clear}

Удаляет все внешние ссылки.

```csharp
public void Clear()
```

### Примечания

При удалении внешних ссылок все формулы, которые ссылаются на них, также будут удалены, потому что ссылки становятся недействительными.

### См. также

* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Clear(bool) {#clear_1}

Удаляет все внешние ссылки.

```csharp
public void Clear(bool updateReferencesAsLocal)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| updateReferencesAsLocal | Boolean | Обновлять ли все ссылки внешних ссылок в формулах на ссылки текущей книги. |

### Примечания

Если требуется обновить ссылки, ссылки внешних ссылок в формулах будут изменены на текущую книгу, когда это возможно. Например, оригинальная формула ячейки выглядит так "='externalsource.xlam'!customfunction()", после удаления внешних ссылок формула станет "=customfunction()"; Когда оригинальная формула выглядит так "='[externalsource.xlam]Sheet1'!$A$1", в зависимости от наличия листа с именем "Sheet1" в текущей книге: если да, формула станет "=Sheet1!$A$1"; если нет, формула станет "=#REF!$A$1". Если обновление ссылок не требуется, все формулы со ссылками на внешние ссылки также будут удалены, поскольку эти ссылки становятся недействительными.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkCollectionMethodClearWithBooleanDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            
            // Добавьте несколько внешних ссылок
            ExternalLinkCollection externalLinks = workbook.Worksheets.ExternalLinks;
            externalLinks.Add("externalWorkbook.xlsx", new string[] { "Sheet1" });
            externalLinks.Add("anotherExternal.xlsx", new string[] { "Sheet1" });
            
            Console.WriteLine("External links count before clear: " + externalLinks.Count);
            
            // Очистить с updateReferences = true
            externalLinks.Clear(true);
            Console.WriteLine("External links count after clear (updateReferences=true): " + externalLinks.Count);
            
            // Снова добавить ссылки
            externalLinks.Add("externalWorkbook.xlsx", new string[] { "Sheet1" });
            externalLinks.Add("anotherExternal.xlsx", new string[] { "Sheet1" });
            
            // Очистить с updateReferences = false
            externalLinks.Clear(false);
            Console.WriteLine("External links count after clear (updateReferences=false): " + externalLinks.Count);
        }
    }
}
```

### См. также

* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


