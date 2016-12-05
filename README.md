# react-native-tips

React Native开启了开发原生App的新方式，不仅提高了开发效率，同时提高了App的用户体验。相比Web App而言，React Native可以使用原生的组件和API，这样就可以释放Native的能力和体验；相比Native开发而言，前端开发者可以使用JavaScript开发原生应用，这样开发效率将会得到很大的提高。

## 目录

### 样式

* `TextInput`设置`lineHeight`无效的时候，需要加上`padding`属性
* 希望元素占满100%高度可以添加`alignSelf: 'stretch'`

### 模拟器

* [开启远程调试后App卡顿主要是因为调试Tab处于后台状态，解决的方法很简单：前置该Tab或者让Tab成为一个独立的窗口](https://github.com/facebook/react-native/issues/10559)
```sh
Remote debugger is in a background tab which may cause apps to perform slowly. Fix this by foregrounding the tab (or opening it in a separate window).
```
