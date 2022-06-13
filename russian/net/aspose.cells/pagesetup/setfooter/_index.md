---
title: SetFooter
second_title: Справочник по Aspose.Cells для .NET API
description: Устанавливает скрипт форматирующий нижний колонтитул файла Excel.
type: docs
weight: 600
url: /ru/net/aspose.cells/pagesetup/setfooter/
---
## PageSetup.SetFooter method

Устанавливает скрипт, форматирующий нижний колонтитул файла Excel.

```csharp
public void SetFooter(int section, string footerScript)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| section | Int32 | 0:Левая секция. |
| footerScript | String | Скрипт формата нижнего колонтитула. |

### Примечания

Команды сценария:

| **Команда**| **Описание**| 
| --- | --- | 
| &amp;P | Текущий номер страницы | 
| &amp;N | Количество страниц | 
| &amp;D | Текущая дата | 
| &amp;T | Текущее время | 
| &amp;A | Имя листа | 
| &amp;F | Имя файла без пути | 
| &amp;"&amp;lt;ИмяШрифта&amp;gt;" | Название шрифта, например:&amp;"Arial" | 
| &amp;"&amp;lt;Название шрифта&amp;gt;, &amp;lt;Стиль шрифта&amp;gt;" | Название и стиль шрифта, например:&amp;"Arial,Bold" | 
| &amp;&amp;lt;Размер шрифта&amp;gt; | Размер шрифта. Если за этой командой следует простое число, которое будет напечатано в заголовке, оно будет отделено от высоты шрифта символом пробела. | 
| &amp;G | Сценарий изображения | 

Например:"&amp;Arial,Bold&amp;8Footer Note"

### Смотрите также

* class [PageSetup](../../pagesetup)
* пространство имен [Aspose.Cells](../../pagesetup)
* сборка [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->