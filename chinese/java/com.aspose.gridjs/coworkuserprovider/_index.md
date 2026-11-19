---
title: "CoWorkUserProvider"
second_title: "Aspose.Cells for Java API 参考"
description: "表示协作模式下的用户提供程序接口。当前仅在 Java 版本可用，未来将在 .netython 版本中提供。"
type: docs
url: /zh/java/com.aspose.gridjs/coworkuserprovider/
---
```
public interface CoWorkUserProvider
```

表示协作模式下的用户提供程序接口。当前仅在 Java 版本可用，未来将在 .net/python 版本中提供。客户应用程序可以实现此接口以提供用户信息。
## 方法

| 方法 | 描述 |
| --- | --- |
| [getCurrentUserId()](#getCurrentUserId--) | 获取当前用户的唯一标识符 |
| [getCurrentUserName()](#getCurrentUserName--) | 获取当前用户的用户名 |
| [getPermission()](#getPermission--) | 获取当前用户的权限级别 |
### getCurrentUserId() {#getCurrentUserId--}
```
public abstract long getCurrentUserId()
```


获取当前用户的唯一标识符

**Returns:**
long - 当前用户 ID
### getCurrentUserName() {#getCurrentUserName--}
```
public abstract String getCurrentUserName()
```


获取当前用户的用户名

**Returns:**
java.lang.String - 当前用户名
### getPermission() {#getPermission--}
```
public abstract int getPermission()
```


获取当前用户的权限级别

**Returns:**
int - [CoWorkUserPermission](../../com.aspose.gridjs/coworkuserpermission)。当前用户权限级别
