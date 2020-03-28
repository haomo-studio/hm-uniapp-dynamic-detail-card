> 官网: [https://haomo-tech.com](https://haomo-tech.com)

> 作者: 毫末科技

> 邮箱: hxg@haomo-studio.com

## 预览

![预览图片](http://downloads.haomo-tech.com/uniapp/hm-dynamic-detail-card.png)

[在线效果预览](http://template.uniapp.haomo-tech.com/pages/haomo/test-component/hm-dynamic-detail-card)

更多毫末科技的uni-app跨端模板，请见[毫末科技uni-app跨端模板](https://haomo-tech.com/sale.html)

## 技术支持

* [uni-app插件市场](https://ext.dcloud.net.cn/plugin?id=1524)

* [npm包](https://www.npmjs.com/package/hm-uniapp-dynamic-detail-card)

* [github地址](https://github.com/haomo-studio/hm-uniapp-dynamic-detail-card)

* [gitee地址](https://gitee.com/haomo/hm-uniapp-dynamic-detail-card)

毫末科技将长期迭代本组件。需要技术支持，请进钉钉群（群号30423559）：

<img width="250" src="http://downloads.haomo-tech.com/%E6%AF%AB%E6%9C%ABuniapp%E7%BB%84%E4%BB%B6%E6%8A%80%E6%9C%AF%E6%94%AF%E6%8C%81.jpg">

## 概述

毫末uni-app毫末动态详情卡片组件。支持H5/小程序(微信、支付宝、头条、百度、QQ)/App；组件可自适应各种屏幕大小的手机。

## 使用

请使用HBuilderX导入组件。

在script中引用：

```javascript
import HmDynamicDetailCard from '@/components/hm-dynamic-detail-card/index.vue'
export default {
    components: { HmDynamicDetailCard }
}
```

在template中使用：

```html
<template>
  <div class="test-component">
    <hm-dynamic-detail-card :options="options"></hm-dynamic-detail-card>
  </div>
</template>
<script>
import HmDynamicDetailCard from '@/components/hm-components/hm-dynamic-detail-card/index.vue'

export default {
  components: { HmDynamicDetailCard },
  data() {
    return {
      options: {
          minutesAgo: '5分钟前',
          name: '张三',
          avator:
            '/static/hm-dynamic-detail-card/images/img_25823_0_3.png',
          introduce: 'xx国际ceo',
          dynamicDetail: '一切尽在计划之中',
          dynamicImage:
            '/static/hm-dynamic-detail-card/images/img_25823_0_4.png',
          submain: '124 喜欢',
          Heart:
            '/static/hm-dynamic-detail-card/images/img_25823_0_2.png',
          messagingspeechbub:
            '/static/hm-dynamic-detail-card/images/img_25823_0_1.png',
          tiaozhuandaomulu:
            '/static/hm-dynamic-detail-card/images/img_25823_0_0.png'
        }
    };
  },
  methods: {
    onClick: function(e) {
      console.log('onClick');
    }
  }
};
</script>
<style>
</style>

```

## 属性说明

| 属性名        | 类型     | 默认值 | 说明                                                                       |
|-----------   |---------|--------|----------------------------------------------------------------------------|
| options        | Object  | -      | 卡片属性                                                                   |

options对象各个属性说明如下：

| 属性名        | 类型     | 默认值 | 说明                                                                       |
|-----------   |---------|--------|----------------------------------------------------------------------------|
| minutesAgo        | String  | -      | 时间                                                                   |
| name        | String  | -      | 姓名                                                                   |
| avator        | String  | -      | 头像                                                                   |
| introduce        | String  | -      | 个人介绍                                                                   |
| dynamicDetail        | String  | -      | 动态详情                                                                   |
| dynamicImage        | String  | -      | 动态图片                                                                   |
| submain        | String  | -      | 喜欢数量                                                                   |
| Heart        | String  | -      | 喜欢图片                                                                   |

## 事件说明

| 事件称名   | 事件说明           | 返回参数 |
|----------|--------------------|----------|
| @click   | 点击 Card 触发事件 | -        |

## 更新日志

### 0.0.1(2020-03-28)

* 完成第一个版本
