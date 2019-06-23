### Material Design - Surface

[TOC]

#### Material Environment

##### The physical world 物理世界

In the physical world, objects can be stacked or attached to one another, but cannot pass through each other. They cast shadows and reflect light.

**在物理世界里，物体能够堆叠或彼此连接，但不能相互穿过。它们投下阴影和反射光线。**

Material Design reflects these qualities in how surfaces are displayed and move across the Material UI. Surfaces, and how they move in three dimensions, are communicated in ways that resemble how they move in the physical world. This spatial model can also be applied consistently across apps.

**Material Design反映了surfaces是如何在Material UI中展示和移动这一方面的这些本质。surfaces以及它们如何在三维空间中移动，其交互通信方式类似于它们在物理世界中的移动方式。这个空间模型也能够跨apps一致地被应用。**

------

##### Depth 深度

Material Design UIs are displayed in an environment that expresses three-dimensional (3D) space using light, surfaces, and cast shadows. All elements in the Material environment move horizontally, vertically, and at varying depths along the z-axis. Depth is depicted by placing elements at various points along the positive z-axis extending towards the viewer.

On the web, the UI expresses 3D space by manipulating the y-axis.

**Material Design UIs在一个通过光线、曲面、投放阴影来表达三维空间的环境中进行渲染展示。在Material环境中的所有元素沿着水平、垂直、通过Z坐标轴的不同深度进行移动。通过将元素放置在沿着正向Z坐标轴的向着观察者扩展的各个点来描述深度。**

**在web中，UI通过操作Y坐标轴来表达三维立体空间。**

------

#### Properties 属性

##### Dimensions 维度

Material has varying x & y dimensions (measured in dp) and a uniform thickness (1dp).

**Material 有很多X和Y维度(用dp作为衡量标准)和一个统一的厚度(1dp)。**

------

##### Shadows 阴影

Material surfaces at different elevations cast shadows.

**Material surfaces在不同的高度中投放的阴影程度也不同。**

------

##### Resolution 分辨率

Material has infinite resolution.

**Material有无限的分辨率。**

------

##### Content 内容(填充物)

Content is displayed in any shape and color on Material. Content does not add thickness to Material. Content is expressed without being a separate layer.

**在Material中，内容能以任何形状和颜色进行展示。内容不会往Material中增加厚度。内容在展示时并不是一个单独的层。**

Content can behave independent of Material, but is limited within the bounds of Material.

**内容的行为能够独立于Material，但是受限于在Material边界内。**

Content behavior can be independent of surface behavior.

**内容的行为可以独立于surface行为。**

Content behavior can depend on Material behavior.

**内容的行为可以依赖于Material行为。**

##### Physical properties 物理属性

Material is solid. User input and interaction cannot pass through material.

**Material是坚固的。用户输入和交互不能穿过material。**

Input events only affect the surface of Material.

**输入事件只能影响Material的表面。**

Material cannot pass through other Material. For example, one Material surface cannot pass through another Material surface when changing elevation.

**Material**不能穿过其他Material。举个例子，当改变Material surface高度时，它不能穿过另一个Material surface。

Material does not behave like a gas.

Material enters and exits through changes in opacity, size, or position.

**Material的行为不会像气体那样。Material进入和退出是通过透明度、尺寸大小或者位置的变化来实现的。**

Material is not fluid like a liquid or gel, though it may display content with these properties.

**Material不像液体或者凝胶那样，虽然它有可能展示一些具有这些特性的内容。**

------

##### Transform Material 转化Material

Material can change shape.

**Material能够改变形状。**

Material can change opacity.

**Material能够改变透明度。**

1. Material can change opacity uniformly across its entire surface. **Material能够透过它完整的surface改变透明度。**
2. Material can change opacity across a portion of its surface. **Material能够透过它部分的surface改变透明。**

Material grows and shrinks only along its plane.

**Material只能沿着其平面延伸或者收缩。**

Material never bends or folds in ways that exceed the depth of the UI.

**Material永远不会以超过UI深度的方式弯曲或折叠。**

Material surfaces can join together to become a single Material surface.

**Material surfaces能够连接在一起成为一个单一的Material surface。**

When split, Material can rejoin. For example, if you remove a portion of Material from a surface, the surface will become whole again.

**拆分时，Material能够重新连接。举个例子，如果从surface移除了Material的一部分，surface会再次成为一个整体。**

Material can split and become whole again. **Material 能够拆分并再次成为整体。**

------

##### Movement 移动

Material can be spontaneously generated or dismissed anywhere in the environment.

**Material能够在环境中的任何地方自发生成或消失。**

Material can move along any axis.

**Material 能够沿着任何的坐标轴移动。**

Material can move along various axises.

**Material能够沿着众多的坐标轴移动。**

Material surfaces can coordinate their motion.

**Material surfaces能否协调它们的移动。**

Material motion along the z-axis is typically a result of user interaction.

**沿着Z轴移动的Material通常是用户交互的结果。**

Material surfaces exhibiting z-axis motion prompted by user interaction.

**通过用户交互促进呈现Z轴移动的Material surfaces。**

#### Attributes

##### Basic Material surface

The basic Material surface is opaque white, with 1dp thickness, and casts a shadow. All UI elements in Material Design result from modifications to this surface.

**Basic Material surface**是不透明的白色，厚度为1dp，并投射出阴影。Material Design里的所有UI元素都是通过对surface修改而产生的。

##### Behavior 行为

Material surfaces can behave in certain ways: 

- **Rigid surfaces** remain the same size through all interactions.
- **Stretchable surfaces** can grow or shrink along one or more edges up to a size limit, then behave as rigid surfaces.
- **Pannable surfaces** remain the same size throughout interactions. They can display additional content upon scrolling within the area, until reaching a content limit. When this limit is reached, they behave as rigid surfaces in that scroll direction.

Material surfaces能够以特定方式呈现：

- 通过所有的相互作用，刚性表面保持同样的尺寸。
- 可拉伸表面可以沿着一个或者多个边缘延伸或收缩直到尺寸限制，然后表现为刚性表面。
- 可交换表面在整个交互过程中保存同样的尺寸大小。它们可以在其区域内滚动时展示额外的内容，直到到达内容限制。当到达这个限制时，它们在滚动方向上表现为刚性表面。

　![](mio-design_assets_19e8l8UXWqC4n_7eMT0d8_YD6CvAwDX-M_materialattributes-stretch-1.mp4)

*Material surface dimensions can grow along one or more axes to accommodate additional content.*

![](./mio-design_assets_1JCxHxRkVWHO_OqZSLar9bIaah5p4yJAk_materialattributes-pan.mp4)

*Material surface dimensions can remain rigid, but content can scroll or pan across the surface.*

###### Composite surfaces

Surfaces can be divided into areas which display different types of behavior.

**Surfaces能够被拆分成多个展示不同类型的行为区域**

![](./mio-design_assets_12LJku-D8qyXCzzx9tH2PVjx73E145zRo_materialattributes-constructingsurfaces-1.mp4)

*A single surface can contain multiple pannable surfaces, such as an embedded map (1) that pans independently of a scrollable list (2).*

![](./mio-design_assets_1lA44inCPDrT5UShoK5fQYynz-KISRSs6_materialattributes-constructingsurfaces-2.mp4)

A card can stretch to display a region that scrolls independently of other card content.

##### Stretchable surfaces  可拉伸的表面

A stretchable surface can be stretched before reaching a limit, at which point the entire surface becomes rigid. Surfaces can stretch vertically, horizontally, or in both directions.

可拉伸的表面能在到达极限之前被拉伸，此时整个表面都会变得刚硬。表面能够被垂直、水平拉伸，或者同时拉伸。

Typically, user interaction with a surface will stretch it in one direction. For example, tapping “more details” can cause a card to grow vertically and display additional content.

通常，用户与表面的交互会在一个方向上延伸。举个例子，点击“more details”会导致卡片沿着垂直方向延伸，并展示额外的内容。

![](./mio-design_assets_1SdOX6Lmt-WHkMKkQ0ySDQmucI7X1oK8X_surfaces-stretchvert.mp4)

Material stretch direction can be exclusively vertical.

![](./mio-design_assets_16aoHYwbnA-hU5bjAUYFWHscqArnDczz9_surfaces-stretchhoriz.mp4)

Material stretch direction can be exclusively horizontal.

Material 延伸的方向也能是水平的。

![](./mio-design_assets_1TMUunFfJc9gZHZGevKpY7l6P142KIC-7_surfaces-stretchverthoriz.mp4)

Material stretch direction can be along both horizontal and vertical axises, either independently or simultaneously.

Material 延伸方向能够同时沿着水平和垂直的坐标轴