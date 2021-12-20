# Uninstall-Edge

https://sspai.com/post/70320

## 三步卸载 Microsoft Edge

1. 管理员模式打开 powershell
2. `cd 'C:\Program Files (x86)\Microsoft\Edge\Application\9*\Installer'`
3. `./setup --uninstall --force-uninstall --system-level`

### 一、管理员模式打开 powershell

在开始菜单搜索 powershell 并右键或直接选择管理员模式打开

<table>
<tr>
<td valign="top" width="50%">

![image](https://user-images.githubusercontent.com/10897528/146189026-64753943-9df8-4ff4-81b5-914d3fc948be.png)

</td>
<td valign="top" width="50%">

![image](https://user-images.githubusercontent.com/10897528/146189958-72f3cdde-7265-46c4-b362-3183c8abcc9f.png)

</td>
</tr>
</table>

### 二、进入 edge Installer 目录

**复制这段内容**，粘贴到 powershell 窗口里（右键即可），回车执行，执行成功会看到提示的前缀有变化：

```powershell
cd 'C:\Program Files (x86)\Microsoft\Edge\Application\9*\Installer'
```

![image](https://user-images.githubusercontent.com/10897528/146190508-346e7814-824a-4f11-a6b8-bfb5acf7358d.png)

---

> 补充说明：
> 
> 这里的通配符 `9*` 是匹配了 edge 的版本号，我本地是 `96.0.1054.57` 版本。所以我最终进入了` C:\Program Files (x86)\Microsoft\Edge\Application\96.0.1054.57\Installer` 目录。

### 三、卸载

**复制这段内容**，粘贴到 powershell 窗口里，回车执行：

```powershell
./setup --uninstall --force-uninstall --system-level
```

效果：![image](https://user-images.githubusercontent.com/10897528/146190998-6a5714b2-06ea-4d2f-bd43-b30b20f8b9e4.png)

## OK，结束了！

你的电脑上不再有 edge 了，再也不会出现这些事情：

1. ![image](https://user-images.githubusercontent.com/10897528/146191371-e94dbe70-b1bc-4deb-9d2c-b2146f89e9dc.png)
2. https://github.com/da2x/EdgeDeflector/issues/141
3. https://zhuanlan.zhihu.com/p/411101495

当然，你还是要手动去设置里把 edge 的默认设置都改成别的浏览器

![image](https://user-images.githubusercontent.com/10897528/146191880-b98d0830-b1bc-4181-a6ce-37ea0699e12c.png)
