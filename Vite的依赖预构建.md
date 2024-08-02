# vite预加载
>在处理的过程中如果说看到了非绝对路径或者相对路径的引入，就会开启路径补全。

```javascript
import_from"lodash";

vite补全的：
import_vite_from"/node_modules/.vite/deps/lodash.js?";
```
找寻依赖的过程是自当前目录一次向上查找的过程，知道搜寻到根目录或者搜寻到对应的依赖为止。

开发环境和生产环境
