# css 长度单位转换器

对传入字符串进行正则替换，可以按顺序执行多个步骤，好用记得 star 哦。
[https://liangwei88.github.io/design-px-convertor/]

## 单位转换
* 一个单位按比例转换为另一个单位，如 16px, 转换为 rem 按照 1 像素等于 0.01 rem 的比值，保留 2 位小数，得出 0.16rem

## 等比数字转换
* 同一个单位相互转换，如 640px 设计稿中的 16px 转换为 750px 设计稿中的数字，保留 0 位小数，得出 19px

## 注意
* 满足下列几种格式，16px; 或 16px 16px 或 16px}
* 即单位后必须带空格或分号或花括号
```
/*错误写法*/
.test {
    width:16px
}

/*正确写法, 三种都可以*/
.test {
    width:16px;
    margin: 16px 22px;
    font-size: 32px}
```