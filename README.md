# JSPrac-menu-silder

### 侧边栏

一.实现思路

主要是css的编写

二.关键知识点

- `z-index: 100; /*层级关系*/`
- `transform: translateX(-100%);隐藏`
- `transform: translateX(200px);向右平移200px` 这里的显示是额昂整个页面向右平移 所以是对body操作
- `transition: transform 0.3s ease; 过渡效果`
- 父相子绝 绝对定位可以使元素脱离文档流，就是它的位置不再是整个相对于整个页面了，而是某个div，从而更方便的调整其位置
- `transform: translate(-50%,- 50%);` 向上偏移50%，向下偏移50%，移动的位置相对于自身而言
- 表单在页面居中 `calc`的用法

    ```
    position: absolute;
    overflow: hidden;
    top:calc(100vh/3);
    left: calc(100%/3);
    ```

- `toggle.addEventListener('click',()=>document.body.classList.toggle('show-nav'))`  通过点击给body设置类名，再次点击清除类名。
- 增加类名：`dom.classList.add('classname')`
- 移除类名：`dom.classList.remove('classname')`
- 动画：淡入淡出效果

    ```jsx
    animation-name:modalopen //动画名
    animation-duration:2s //动画持续时间

    @keyframes modalopen{
    	from{
    		opacity:0;
    	}
    	to{
    		opacity:1;
    	}
    }
    ```

