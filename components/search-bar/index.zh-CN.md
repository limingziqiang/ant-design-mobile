---
category: Components
type: Data Entry
title: SearchBar
subtitle: 搜索栏
---

一般可位于 NavBar 下方，通过『取消按钮』退出激活状态。

### 规则

- 应该在 placeholder 里提供提示文字，提醒用户输入相关内容，比如：双11特卖。
- 在搜索栏下方，可提供有用的标签文案，帮助用户通过点击直接完成输入，比如：列出一些最近搜索的关键词。

## API

适用平台：WEB、React-Native

属性 | 说明 | 类型 | 默认值
----|-----|------|------
| defaultValue |    搜索框的默认值     | String |    |
| value      |  搜索框的当前值  | String |    |
| placeholder    |    placeholder     | String |    |
| onSubmit    |  submit 事件 (点击键盘的 enter)  | (val: string): void |    |
| onChange    |    change 事件的回调     | (val: string): void |    |
| onFocus    |    focus 事件的回调     | (): void |    |
| onBlur    |    blur 事件的回调     | (): void |    |
| onCancel  | 点击`取消`按钮触发 (不再自动清除输入框的文字) | (val: string): void |    |
| showCancelButton    |    是否一直显示`取消`按钮     | bool |  `false`  |
| cancelText    |   定制`取消`按钮的文字     | String |  `取消`  |
| disabled    |  设置禁用   | bool |  `false`  |
| onClear(`web only`)    |    点击 clear 图标触发  | (val: string): void |    |
| autoFocus(`web only`)   | 页面初始化时`SearchBar`自动获取光标, 每个页面只有一个`SearchBar`的`autoFocus`会生效 (不保证兼容所有浏览器，目前只支付宝客户端支持) | bool | false  |
| focused(`web only`)   | 手动聚焦 SearchBar (在`focused`设置为 true 后，需要在`onFocus`或者`onBlur`时再次将该属性设置为 false ) | bool | false  |

注：RN 版本更多 API 请参考 [http://facebook.github.io/react-native/docs/textinput.html](http://facebook.github.io/react-native/docs/textinput.html)
