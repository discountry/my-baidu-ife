---
layout: post
title:  WebGL No.1 - Three.js 入门
categories: threejs
---

## Lesson

* [WebGL No.1 - Three.js 入门](http://ife.baidu.com/course/detail/id/18)

## References

* [图灵社区-Three.js入门指南](http://www.ituring.com.cn/book/1272)
* [Github-《Three.js 入门指南》书例代码](https://github.com/Ovilia/ThreeExample.js)
* [在线电子书-ThreeExamples.js](http://zhangwenli.com/ThreeExample.js/)
* [Three.js官网文档](https://threejs.org/docs/index.html#Manual/Getting_Started/Creating_a_scene)

## Demo

* [LearnThreeJS Collection On Codepen](http://codepen.io/collection/DYGjeo/)

## Task

* [ThreeJS-Car preview](http://codepen.io/discountry/pen/aJbejg?editors=0010)
* [ThreeJS-Car source code](https://github.com/discountry/my-baidu-ife/blob/master/codes/Misc/threejs-car.html)

**html**

```html
<canvas id="mainCanvas" width="800px" height="600px"></canvas>
```

**js**

```js
var renderer = new THREE.WebGLRenderer({
  canvas: document.getElementById('mainCanvas')
});

renderer.setClearColor(0x000000);

var scene = new THREE.Scene();

//THREE.OrthographicCamera(left, right, top, bottom, near, far)
var camera = new THREE.OrthographicCamera(-10, 30, 20, -10, 0.1, 100);
camera.position.set(25, 25, 35);
camera.lookAt(new THREE.Vector3(0, 0, 0));
scene.add(camera);

var light = new THREE.PointLight(0xffffff, 2, 100);
light.position.set(15, 25, 25);
scene.add(light);

//THREE.TorusGeometry(radius, tube, radialSegments, tubularSegments, arc)
var torus = new THREE.Mesh(new THREE.TorusGeometry(2, 1, 12, 18),
  new THREE.MeshLambertMaterial({
    color: 0xffffff
  }));
scene.add(torus);

var torus2 = new THREE.Mesh(new THREE.TorusGeometry(2, 1, 12, 18),
  new THREE.MeshLambertMaterial({
    color: 0xffffff
  }));
//Move geometry to other coordinates.
torus2.position.set(10, 0, 0)
scene.add(torus2);

//THREE.CubeGeometry(width, height, depth, widthSegments, heightSegments, depthSegments)
var box = new THREE.Mesh(new THREE.BoxGeometry(18, 10, 10), new THREE.MeshLambertMaterial({
  color: 0xffffff
}));
box.position.set(5, 5, -5)
scene.add(box);

renderer.render(scene, camera);
```

## Note

**正交vs透视(Orthographic&perspective)**

![pvso](https://ooo.0o0.ooo/2017/02/24/58b04ba380b4d.png)


