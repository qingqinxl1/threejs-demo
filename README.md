1. 全局安装node-http
`npm install http-server -g`
2. 该项目目录下开启服务
`http-server . -p 8000`
3. three.js常用功能
### 照相机
> 正交投影照相机

`new THREE.OrthographicCamera(-2, 2, 1.5, -1.5, 1, 10);`

> 透视投影照相机

`new THREE.PerspectiveCamera(45, 400 / 300, 1, 10);`

### 几何形状
> 立方体

`THREE.CubeGeometry(width, height, depth, widthSegments, heightSegments, depthSegments)`

> 球体

`THREE.SphereGeometry(radius, segmentsWidth, segmentsHeight, phiStart, phiLength, thetaStart, thetaLength)`

> 文字形状

> 自定义形状

*另外还有圆柱体、正四面体、正八面体、正十二面体、圆环圈（甜甜圈的形状）、圆环结等*

### 材质
> 基本材质

`THREE.MeshBasicMaterial(opt)`

> lambert材质

```javascript
new THREE.MeshLambertMaterial({
    color: 0xffff00,
    emissive: 0xff0000
})
```

> phong材质

```javascript
material = new THREE.MeshPhongMaterial({
    color: 0xff0000,
    specular: 0xffff00,
    shininess: 100
});
```

> 法相材质

`new THREE.MeshNormalMaterial()`

### 网格
> 创建网格

`Mesh(geometry, material)`

### 参考文档
[three.js入门指南](https://read.douban.com/reader/ebook/7412854/)