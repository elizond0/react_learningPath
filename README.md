# react_learningPath

## 0.简介

* React起源于Facebook的内部项目，该公司积极尝试引入HTML5技术用来架设Instagram网站，开发中发现HTML5的性能下降明显，达不到预期的效果，就自己开发了React框架。
* 特点:
1. 虚拟DOM: React也是以数据驱动的，每次数据变化React都会扫瞄整个虚拟DOM树，自动计算与上次虚拟DOM的差异变化，然后针对需要变化的部分进行实际的浏览器DOM更新
2. 组件化： React可以从功能角度横向划分，将UI分解成不同组件，各组件都独立封装，整个UI是由一个个小组件构成的一个大组件，每个组件只关系自身的逻辑，彼此独立
3. 单项数据流：React设计者认为数据双向绑定虽然便捷，但在复杂场景下副作用也是很明显，所以React更倾向于单向的数据流动-从父节点传递到子节点。（使用ReactLink也可以实现双向绑定，但不建议使用）

## 1.基础环境
* html中引入react.js和react-dom.js文件即构成基础环境
* React.createClass注册一个组件类,通过调用React.createElement('h1', null, 'Hello')生成html内容
* ReactDOM.render是React的最基本方法，用于将模板转为HTML语言，并插入指定的DOM节点