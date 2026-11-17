---
title: "Класс LowCodePdfSaveOptions"
linktitle: "LowCodePdfSaveOptions"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс LowCodePdfSaveOptions. Инкапсулирует объект, представляющий lowcodepdfsaveoptions в Go."
type: docs
weight: 200
url: /ru/go-cpp/lowcodepdfsaveoptions/
---

## LowCodePdfSaveOptions class

Параметры сохранения PDF в режиме low code.

```go

type LowCodePdfSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewLowCodePdfSaveOptions](./newlowcodepdfsaveoptions/) | Конструктор по умолчанию. |
| [NewLowCodePdfSaveOptions_LowCodeSaveOptions](./newlowcodepdfsaveoptions_lowcodesaveoptions/) | Создаётся из родительского объекта. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetSaveFormat](./getsaveformat/) | Формат сохранения для вывода. При конвертации в pdf может быть только SaveFormat.Pdf. |
| [SetSaveFormat](./setsaveformat/) | Формат сохранения для вывода. При конвертации в pdf может быть только SaveFormat.Pdf. |
| [GetPdfOptions](./getpdfoptions/) | Опции для сохранения PDF-файла. |
| [SetPdfOptions](./setpdfoptions/) | Опции для сохранения PDF-файла. |
| [GetOutputFile](./getoutputfile/) | Получает и задает файл(с путём, если необходимо) для сохранения сгенерированных данных. При установке этого свойства значением, отличным от null или пустой строки, OutputStream будет игнорироваться. |
| [SetOutputFile](./setoutputfile/) | Получает и задает файл(с путём, если необходимо) для сохранения сгенерированных данных. При установке этого свойства значением, отличным от null или пустой строки, OutputStream будет игнорироваться. |
| [GetOutputStream](./getoutputstream/) | Получает и задает поток для записи сгенерированных данных. При установке этого свойства значением, отличным от null, OutputFile будет игнорироваться. |
| [SetOutputStream](./setoutputstream/) | Получает и задает поток для записи сгенерированных данных. При установке этого свойства значением, отличным от null, OutputFile будет игнорироваться. |
