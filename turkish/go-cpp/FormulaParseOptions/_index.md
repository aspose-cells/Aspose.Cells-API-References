---
title: "FormulaParseOptions Sınıfı"
linktitle: "FormulaParseOptions"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "FormulaParseOptions sınıfı. Go'da formulaparseoptions'ı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/formulaparseoptions/
---

## FormulaParseOptions class

Formül ayrıştırılırken seçenekleri temsil eder.

```go

type FormulaParseOptions struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewFormulaParseOptions](./newformulaparseoptions/) | Varsayılan yapıcı. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetLocaleDependent](./getlocaledependent/) | Formülün yerel ayarlara göre biçimlendirilip biçimlendirilmediği. Varsayılan değer false. |
| [SetLocaleDependent](./setlocaledependent/) | Formülün yerel ayarlara göre biçimlendirilip biçimlendirilmediği. Varsayılan değer false. |
| [GetR1C1Style](./getr1c1style/) | Formülün R1C1 referans stilinde olup olmadığı. Varsayılan değer false. |
| [SetR1C1Style](./setr1c1style/) | Formülün R1C1 referans stilinde olup olmadığı. Varsayılan değer false. |
| [GetCheckAddIn](./getcheckaddin/) | Mevcut çalışma kitabının mevcut dış bağlantılarında dış bağlantısı olmayan kullanıcı tanımlı işlev için eklentileri kontrol edip etmeyeceği. Varsayılan değer true (eğer kullanıcı tanımlı işlev mevcut dış bağlantılardaki bir eklentiyle eşleşirse, o eklenti olarak kabul edilir). |
| [SetCheckAddIn](./setcheckaddin/) | Mevcut çalışma kitabının mevcut dış bağlantılarında dış bağlantısı olmayan kullanıcı tanımlı işlev için eklentileri kontrol edip etmeyeceği. Varsayılan değer true (eğer kullanıcı tanımlı işlev mevcut dış bağlantılardaki bir eklentiyle eşleşirse, o eklenti olarak kabul edilir). |
| [GetParse](./getparse/) | Verilen formülün ayrıştırılıp ayrıştırılmayacağı. Varsayılan değer true. False ise, verilen formül dizesi hücrede olduğu gibi tutulur ve kullanıcı diğer yöntemleri çağırıp ayrıştırana kadar ya da ayrıştırılmış formül verileri formüllerin hesaplanması gibi diğer işlemler için gerektiğinde kullanılmaz. |
| [SetParse](./setparse/) | Verilen formülün ayrıştırılıp ayrıştırılmayacağı. Varsayılan değer true. False ise, verilen formül dizesi hücrede olduğu gibi tutulur ve kullanıcı diğer yöntemleri çağırıp ayrıştırana kadar ya da ayrıştırılmış formül verileri formüllerin hesaplanması gibi diğer işlemler için gerektiğinde kullanılmaz. |
| [GetCustomFunctionDefinition](./getcustomfunctiondefinition/) | Özel işlevlerin ayrıştırılması için tanım. |
| [SetCustomFunctionDefinition](./setcustomfunctiondefinition/) | Özel işlevlerin ayrıştırılması için tanım. |
