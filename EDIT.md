# edit

## 新增 match taskNameTemplate 两个配置

* 新增 match 配置（只加载目录中和 match 匹配的 js）
* 新增 taskNameTemplate 配置

```javascript
gulpRequireTasks({
  path: process.cwd() + '/../assets/',
  separator: ':',
  passGulp: true,
  passCallback: true,
  gulp: gulp,
  match: /gulpmodule.js$/,
  taskNameTemplate: 'resources/assets/###.js'
});
```
