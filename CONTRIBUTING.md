# CONTRIBUTING Guide

## 如何贡献

直接修改/添加做菜指南并提交 Pull request 即可。

在写新菜谱时，请复制并修改已有的模板: [示例菜](./dishes/template/示例菜/示例菜.md)。

记得在提交 Pull Request 前同样更新一下 README.md 里的引用。

## 内容规范

**菜谱提交者无需阅读此内容规范。以下内容已经以简明易懂的方式包含在示例模板中。项目的维护者会在你的PR中提出建议, 并协助修改。**

本项目的 Motivation 要求菜谱满足以下规范，不符合规范的菜谱将不会被合并到代码库中。项目的维护者维护此文档, 作为正式的标准与共识。

1. 每一道菜谱至少应包含`原材料与工具`, `计算`, `操作`三部分内容。

`原材料与工具`应列出本菜品需要的除`假想已准备好的物品`外的所有原材料与厨具。
`计算`应定量列出本菜品所需的原材料的量。（无论与人数是否相关）
`操作`应说明菜品的制作步骤。

2. 菜品的制作步骤应当明确(无歧义,non-ambiguous)，并尽可能准确(accurate)。有歧义(ambiguous)的描述是不可接受的，而不准确(inaccurate)或不精确(imprecise)的描述是可以接受的。

> 不准确的菜谱会导致菜品口味有少许偏差，不明确的菜谱会导致做菜人的心态有明显不安。

举例：有歧义的描述

```
# 解释：此处对于盐量的描述是有歧义的。
#       因为对于某个数量的盐，用户无法得出确定的客观结论：此数量是否属于"少量"。
加入少量盐

加入几滴蚝油
将锅加热至八分热
撒上少许葱花
煮至鸡肉断生
```

举例：无歧义的描述

```
# 解释：此处对于锅的温度的描述是不准确的（可能是200摄氏度左右的任何温度），但这个描述是无歧义的。
#       因为对于锅的某个状态，用户可以进行水滴测试，并得出确定的客观结论：此状态要么符合要求，要么不符合要求。
加热锅，直至"滴入几滴水时，水珠能够在锅上迅速滚动而不吸附"
加热锅，直至观察到莱顿弗罗斯特现象

加入5ml酱油
等到水沸腾后
继续煮，直到汤汁剩下二分之一
煎至表面呈金黄色
继续翻炒两分钟

# 食材所可能粘附的蛋液的量是确定的
裹上蛋液

# 在'计算'中已提及将用到葱花的量
撒上葱花
```

考虑到现实因素，对于某些在家庭厨房中确实难以明确描述的因素，可以作为特例排除。例如

```
# 在描述燃气灶火焰强度时
文火, 小火, 中火, 大火 等
# 在描述颜色时
金黄色 等
# 在描述硬度时
变软 变硬
```

3. 菜品的`制作步骤`应当完整(complete)。这意味着, 在执行完所有操作步骤后, 菜品已经被完成。

4. 菜品的`原材料与工具`应当完整(complete)。这意味着, 在执行操作步骤时, 没有用到`原材料与工具`中未提到的物品。

## 审核员须知

下面的内容仅供参与菜谱审批的人员参考。

审批时，最重要的是避免歧义：保证按照他的菜谱尽可能没有灵活发挥空间。所有歧义都要指出。就是，无论是个大厨还是个萌新，只要按照菜谱，做出来的效果应该完全一样。

- 绝对不允许菜谱中出现灵活发挥的空间。不允许让厨师自己斟酌加入的量。不允许出现 `适量` `少量`
- 针对单个大小体积重量差距极大的物体，不允许用个来约束，要额外标注重量 g
- 勺 不是一个可靠的单位。建议换成毫升 ml
- 对蒜的描述，指的是三头还是三瓣可能产生歧义
- 允许出现 `大火` `中火` `小火`
- 任何标点符号，例如顿号，都需要额外确认是否是`可以替代的或`，还是`必须同时添加的和`
- 如果一个原材料仅仅计算了一次，而引用了多次，必须额外确认每次引用时指的量的多少
- 确保他在合并前更新了 Readme 对他的菜谱的引用，如果他是在新加菜谱的话
- 确保他没有破坏模板的一二级标题格式
- 确保他没有删除模板中必需的内容
- 确保他删除干净了模板里的注释
- 确保分类正确，不和已有的菜名重复