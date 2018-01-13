# wepy-com-selectab

[![NPM](https://nodei.co/npm/wepy-com-selectab.png)](https://nodei.co/npm/wepy-com-selectab/)

> 适用于选座位等数字或者类型选择的组件，这是一个从`Bandix`独立出来的组件。

早期Vue实现版本（异曲同工）：[https://github.com/ColMugX/vue-number-tab](https://github.com/ColMugX/vue-number-tab)

![](https://github.com/ColMugX/vue-number-tab/raw/master/screenshots/1.gif)

## 安装 Install

> npm install -S wepy-com-selectab

## 使用 Usage

```js
import Selectab from 'wepy-com-selectab'

export ...

    components = {
        selectab: Selectab
    }
```

```vue
<selectab :total.sync="total" :value="value" bgColor="#444751" @selected="handleSelected" />
```
默认是选择数字，从`1`到`4`，颜色是`#444751`

## 配置 Options

### Api

| 参数       | 说明               | 类型              | 可选值         | 默认值     |
| -------- | ---------------- | --------------- | ----------- | ------- |
| total    | 数字的总数，或者通过数组传入数据 | [Array] | -           | [1, 2, 3, 4]       |
| value    | 组件默认选择数据         | [String]        | -           | 1       |
| bgColor  | 选择区块颜色           | String          | -           | #444751 |

### Event

| 参数        | 说明       | 返回值              |
| --------- | -------- | ---------------- |
| selected | 获取当前选择数据 | [String] |
