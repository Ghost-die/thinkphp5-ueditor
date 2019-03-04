
#### 初始化项目资源
  > 在项目目录下面找到 command.php 添加控制台添加下面配置
```
    return [
        'ghost\uedit\Edit'
    ];
  
```
  > 执行console命令初始化assets资源 
```
    php think editbuild   ##默认资源目录
    php think editbuild --path /src/path   ##绝对路径
    php think editbuild --path admin/js   ##默认资源目录下面的路径
  
```
 > 执行console命令初始化config配置
```
    php think editbuild --config y   ##初始化config配置
```
> 前台使用方式
```
<div>
    {:build_editor(['name'=>'content','content'=>''])}
    <textarea name="content" id="content"></textarea>
</div>
```