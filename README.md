<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8" />
        <title></title>
        <script src="https://aframe.io/releases/0.2.0/aframe.js"></script>
        <script src="https://rawgit.com/ngokevin/aframe-layout-component/master/dist/aframe-layout-component.min.js"></script>
        <!-- Drop in another component and use it from markup. -->
        <script src="https://rawgit.com/ngokevin/aframe-template-component/master/dist/aframe-template-component.min.js"></script>
    </head>
    <body>

<a-scene>

  <a-assets>

    <!-- Platform au centre -->

    <script id="platform" type="text/x-nunjucks-template">
    <a-entity layout="type: circle; radius: 6" position="0 0 -15" rotation="0 0 0">

    {% for x in range(num) %}

    <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 3; depth: 5" rotation="0 180 0"
              material="side: double; color: #00695c"></a-entity>

    <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 3; depth: 5" rotation="0 90 0"
              material="side: double; color: #00695c"></a-entity>

    <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 3; depth: 5" rotation="0 0 0"
              material="side: double; color: #00695c"></a-entity>


    <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 3; depth: 5" rotation="0 -90 0"
              material="side: double; color: #00695c"></a-entity>


    {% endfor %}
    </a-entity>
    </script>

    <script id="platform2" type="text/x-nunjucks-template">
    <a-entity layout="type: circle; radius: 6" position="6 3 -15" rotation="0 45 0">

    {% for x in range(num) %}

    <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 3; depth: 5" rotation="0 180 0"
              material="side: double; color: #FFF"></a-entity>

    <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 3; depth: 5" rotation="0 90 0"
              material="side: double; color: #FF5722"></a-entity>

    <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 3; depth: 5" rotation="0 0 0"
              material="side: double; color: #FFF"></a-entity>


    <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 3; depth: 5" rotation="0 -90 0"
              material="side: double; color: #FF5722"></a-entity>


    {% endfor %}
    </a-entity>

    </script>


    <script id="platform3" type="text/x-nunjucks-template">
    <a-entity layout="type: circle; radius: 16" position="0 0 -15" rotation="0 0 0">

    {% for x in range(num) %}

    <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 3; depth: 5" rotation="0 180 0"
              material="side: double; color: #FF5B2B"></a-entity>

    <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 3; depth: 5" position="0 0 90" rotation="0 90 0"
              material="side: double; color: #B1221C"></a-entity>

    <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 3; depth: 5" rotation="0 0 0"
              material="side: double; color: #34393E"></a-entity>


    <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 3; depth: 5" rotation="0 -90 0"
              material="side: double; color: #FFDA8C"></a-entity>


    {% endfor %}
    </a-entity>
    </script>

    <script id="platform4" type="text/x-nunjucks-template">
    <a-entity layout="type: circle; radius: 8" position="6 2 -15" rotation="0 45 0">

    {% for x in range(num) %}

    <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 3; depth: 5" rotation="0 180 0"
              material="side: double; color: #01579B"></a-entity>

    <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 3; depth: 5" rotation="0 90 0"
              material="side: double; color: #FF8A65"></a-entity>

    <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 3; depth: 5" rotation="0 0 0"
              material="side: double; color: #01579B"></a-entity>


    <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 3; depth: 5" rotation="0 -90 0"
              material="side: double; color: #9C27B0"></a-entity>


    {% endfor %}
    </a-entity>
    </script>

    <script id="platform5" type="text/x-nunjucks-template">
    <a-entity layout="type: circle; radius: 12" position="6 1 -15" rotation="0 45 0">

    {% for x in range(num) %}

    <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 3; depth: 5" rotation="0 180 0"
              material="side: double; color: #E91E63"></a-entity>

    <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 3; depth: 5" rotation="0 90 0"
              material="side: double; color: #558B2F"></a-entity>

    <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 3; depth: 5" rotation="0 0 0"
              material="side: double; color: #FFB74D"></a-entity>


    <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 3; depth: 5" rotation="0 -90 0"
              material="side: double; color: #00695C"></a-entity>


    {% endfor %}
    </a-entity>
    </script>

    <script id="platform6" type="text/x-nunjucks-template">
      <a-entity layout="type: circle; radius: 1" position="6 4 -15" rotation="0 45 0">

        {% for x in range(num) %}

        <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 3; depth: 5" rotation="0 0 0"
                  material="side: double; color: #FFB74D"></a-entity>
        <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 3; depth: 5" rotation="0 0 0"
                  material="side: double; color: #FFB74D"></a-entity>
        <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 3; depth: 5" rotation="0 0 0"
                  material="side: double; color: #FFB74D"></a-entity>
        <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 3; depth: 5" rotation="0 0 0"
                  material="side: double; color: #FFB74D"></a-entity>


        {% endfor %}
      </a-entity>
    </script>

    <script id="platform7" type="text/x-nunjucks-template">
      <a-entity layout="type: circle; radius: 18" position="6 4 -15" rotation="0 45 0">

        {% for x in range(num) %}

        <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 1; depth: 5" rotation="0 90 0"
                  material="side: double; color: #FFB74D"></a-entity>
        <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 5; depth: 5" rotation="0 60 0"
                  material="side: double; color: #FFB74D"></a-entity>
        <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 1; depth: 5" rotation="0 60 0"
                  material="side: double; color: #FFB74D"></a-entity>
        <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 1; depth: 5" rotation="0 140 0"
                  material="side: double; color: #FFB74D"></a-entity>


        {% endfor %}
      </a-entity>
    </script>


    <script id="platform8" type="text/x-nunjucks-template">
      <a-entity layout="type: circle; radius: 18" position="6 2 -15" rotation="0 45 0">

        {% for x in range(num) %}

        <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 1; depth: 5" rotation="0 90 0"
                  material="side: double; color: #388E3C"></a-entity>
        <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 5; depth: 5" rotation="0 60 0"
                  material="side: double; color: #388E3C"></a-entity>
        <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 1; depth: 5" rotation="0 60 0"
                  material="side: double; color: #388E3C"></a-entity>
        <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 1; depth: 5" rotation="0 140 0"
                  material="side: double; color: #388E3C"></a-entity>


        {% endfor %}
      </a-entity>
    </script>
    <!-- Fin platform centrale -->

    <!-- Platform de droite -->
    <script id="platform9" type="text/x-nunjucks-template">
    <a-entity layout="type: circle; radius: 12" position="0 0 -15" rotation="0 0 0">

    {% for x in range(num) %}

    <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 2; depth: 5" rotation="0 180 0"
              material="side: double; color: #00695c"></a-entity>

    <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 3; depth: 5" rotation="0 90 0"
              material="side: double; color: #00695c"></a-entity>

    <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 1; depth: 5" rotation="0 0 0"
              material="side: double; color: #00695c"></a-entity>


    <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 2; depth: 5" rotation="0 -90 0"
              material="side: double; color: #00695c"></a-entity>


    {% endfor %}
    </a-entity>
    </script>

    <script id="platform10" type="text/x-nunjucks-template">
    <a-entity layout="type: circle; radius: 6" position="6 3 -15" rotation="0 45 0">

    {% for x in range(num) %}

    <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 3; depth: 5" rotation="0 180 0"
              material="side: double; color: #FFF"></a-entity>

    <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 3; depth: 5" rotation="0 90 0"
              material="side: double; color: #FF5722"></a-entity>

    <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 3; depth: 5" rotation="0 0 0"
              material="side: double; color: #FFF"></a-entity>


    <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 3; depth: 5" rotation="0 -90 0"
              material="side: double; color: #FF5722"></a-entity>


    {% endfor %}
    </a-entity>

    </script>


    <script id="platform11" type="text/x-nunjucks-template">
    <a-entity layout="type: circle; radius: 20" position="0 0 -15" rotation="0 0 0">

    {% for x in range(num) %}

    <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 1; depth: 5" rotation="0 180 0"
              material="side: double; color: #FF5B2B"></a-entity>

    <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 1; depth: 5" position="0 0 90" rotation="0 90 0"
              material="side: double; color: #B1221C"></a-entity>

    <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 2; depth: 5" rotation="0 0 0"
              material="side: double; color: #34393E"></a-entity>


    <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 3; depth: 5" rotation="0 -90 0"
              material="side: double; color: #FFDA8C"></a-entity>


    {% endfor %}
    </a-entity>
    </script>

    <script id="platform12" type="text/x-nunjucks-template">
    <a-entity layout="type: circle; radius: 18" position="6 2 -15" rotation="0 45 0">

    {% for x in range(num) %}

    <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 2; depth: 5" rotation="0 180 0"
              material="side: double; color: #01579B"></a-entity>

    <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 1; depth: 5" rotation="0 90 0"
              material="side: double; color: #FF8A65"></a-entity>

    <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 3; depth: 5" rotation="0 0 0"
              material="side: double; color: #01579B"></a-entity>


    <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 1; depth: 5" rotation="0 -90 0"
              material="side: double; color: #9C27B0"></a-entity>


    {% endfor %}
    </a-entity>
    </script>

    <script id="platform13" type="text/x-nunjucks-template">
    <a-entity layout="type: circle; radius: 16" position="6 1 -15" rotation="0 45 0">

    {% for x in range(num) %}

    <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 3; depth: 5" rotation="0 180 0"
              material="side: double; color: #E91E63"></a-entity>

    <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 1; depth: 5" rotation="0 90 0"
              material="side: double; color: #558B2F"></a-entity>

    <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 1; depth: 5" rotation="0 0 0"
              material="side: double; color: #FFB74D"></a-entity>


    <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 3; depth: 5" rotation="0 -90 0"
              material="side: double; color: #00695C"></a-entity>


    {% endfor %}
    </a-entity>
    </script>

    <script id="platform14" type="text/x-nunjucks-template">
      <a-entity layout="type: circle; radius: 8" position="6 8 -15" rotation="0 45 0">

        {% for x in range(num) %}

        <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 8; width: 3; depth: 5" rotation="0 0 0"
                  material="side: double; color: #FFB74D"></a-entity>
        <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 8; width: 3; depth: 5" rotation="0 0 0"
                  material="side: double; color: #FFB74D"></a-entity>
        <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 8; width: 3; depth: 5" rotation="0 0 0"
                  material="side: double; color: #FFB74D"></a-entity>
        <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 8; width: 3; depth: 5" rotation="0 0 0"
                  material="side: double; color: #FFB74D"></a-entity>


        {% endfor %}
      </a-entity>
    </script>

    <script id="platform15" type="text/x-nunjucks-template">
      <a-entity layout="type: circle; radius: 18" position="6 4 -15" rotation="0 45 0">

        {% for x in range(num) %}

        <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 1; depth: 5" rotation="0 90 0"
                  material="side: double; color: #FFB74D"></a-entity>
        <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 5; depth: 5" rotation="0 60 0"
                  material="side: double; color: #FFB74D"></a-entity>
        <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 1; depth: 5" rotation="0 60 0"
                  material="side: double; color: #FFB74D"></a-entity>
        <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 1; depth: 5" rotation="0 140 0"
                  material="side: double; color: #FFB74D"></a-entity>


        {% endfor %}
      </a-entity>
    </script>


    <script id="platform16" type="text/x-nunjucks-template">
      <a-entity layout="type: circle; radius: 25" position="6 2 -15" rotation="0 45 0">

        {% for x in range(num) %}

        <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 1; depth: 5" rotation="0 90 0"
                  material="side: double; color: #388E3C"></a-entity>
        <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 5; depth: 5" rotation="0 60 0"
                  material="side: double; color: #388E3C"></a-entity>
        <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 1; depth: 5" rotation="0 60 0"
                  material="side: double; color: #388E3C"></a-entity>
        <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 1; depth: 5" rotation="0 140 0"
                  material="side: double; color: #388E3C"></a-entity>


        {% endfor %}
      </a-entity>
    </script>

    <script id="platform16B" type="text/x-nunjucks-template">
      <a-entity layout="type: circle; radius: 5" position="6 1 -15" rotation="0 45 0">

        {% for x in range(num) %}

        <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 1; depth: 5" rotation="0 90 0"
                  material="side: double; color: #FFF"></a-entity>
        <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 5; depth: 5" rotation="0 60 0"
                  material="side: double; color: #FFF"></a-entity>
        <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 1; depth: 5" rotation="0 60 0"
                  material="side: double; color: #FFF"></a-entity>
        <a-entity geometry="primitive: box; openEnded: false; thetaLength: 180; height: 0.3; width: 1; depth: 5" rotation="0 140 0"
                  material="side: double; color: #FFF"></a-entity>


        {% endfor %}
      </a-entity>
    </script>
    <!-- Fin platform de droite -->

  </a-assets>

<a-entity position="0 0 0">
  <a-entity template="src: #platform" data-num="1"></a-entity>
  <a-entity template="src: #platform2" data-num="1"></a-entity>
  <a-entity template="src: #platform3" data-num="3"></a-entity>
  <a-entity template="src: #platform4" data-num="2"></a-entity>
  <a-entity template="src: #platform5" data-num="3"></a-entity>
  <a-entity template="src: #platform6" data-num="1"></a-entity>
  <a-entity template="src: #platform7" data-num="2"></a-entity>
  <a-entity template="src: #platform8" data-num="3"></a-entity>
</a-entity>

<a-entity position="50 0 0">
  <a-entity template="src: #platform" data-num="1"></a-entity>
  <a-entity template="src: #platform2" data-num="1"></a-entity>
  <a-entity template="src: #platform3" data-num="3"></a-entity>
  <a-entity template="src: #platform4" data-num="2"></a-entity>
  <a-entity template="src: #platform5" data-num="3"></a-entity>
  <a-entity template="src: #platform6" data-num="1"></a-entity>
  <a-entity template="src: #platform7" data-num="2"></a-entity>
  <a-entity template="src: #platform8" data-num="3"></a-entity>
</a-entity>

<a-entity position="40 0 0">
  <a-entity template="src: #platform9" data-num="2"></a-entity>
  <a-entity template="src: #platform10" data-num="1"></a-entity>
  <a-entity template="src: #platform11" data-num="3"></a-entity>
  <a-entity template="src: #platform12" data-num="3"></a-entity>
  <a-entity template="src: #platform13" data-num="4"></a-entity>
  <!-- <a-entity template="src: #platform14" data-num="16"></a-entity> -->
  <a-entity template="src: #platform15" data-num="2"></a-entity>
  <a-entity template="src: #platform16" data-num="3"></a-entity>
  <a-entity template="src: #platform16B" data-num="3"></a-entity>
</a-entity>

<a-entity position="40 13 0">
  <a-entity template="src: #platform9" data-num="2"></a-entity>
  <a-entity template="src: #platform10" data-num="1"></a-entity>
  <a-entity template="src: #platform11" data-num="3"></a-entity>
  <a-entity template="src: #platform12" data-num="3"></a-entity>
  <a-entity template="src: #platform13" data-num="4"></a-entity>
  <a-entity template="src: #platform14" data-num="16"></a-entity>
  <a-entity template="src: #platform15" data-num="2"></a-entity>
  <a-entity template="src: #platform16" data-num="3"></a-entity>
  <a-entity template="src: #platform16B" data-num="3"></a-entity>
</a-entity>

<!--  -->

    <a-entity position="40 0 100">
      <a-entity template="src: #platform9" data-num="2"></a-entity>
      <a-entity template="src: #platform10" data-num="1"></a-entity>
      <a-entity template="src: #platform11" data-num="3"></a-entity>
      <a-entity template="src: #platform12" data-num="3"></a-entity>
      <a-entity template="src: #platform13" data-num="4"></a-entity>
      <a-entity template="src: #platform15" data-num="2"></a-entity>
      <a-entity template="src: #platform16" data-num="3"></a-entity>
      <a-entity template="src: #platform16B" data-num="3"></a-entity>
    </a-entity>

    <a-entity position="40 13 100">
      <a-entity template="src: #platform9" data-num="2"></a-entity>
      <a-entity template="src: #platform10" data-num="1"></a-entity>
      <a-entity template="src: #platform11" data-num="3"></a-entity>
      <a-entity template="src: #platform12" data-num="3"></a-entity>
      <a-entity template="src: #platform13" data-num="4"></a-entity>
      <a-entity template="src: #platform15" data-num="2"></a-entity>
      <a-entity template="src: #platform16" data-num="3"></a-entity>
      <a-entity template="src: #platform16B" data-num="3"></a-entity>
    </a-entity>

    <!-- TEST -->

    <a-entity position="50 20 100">
      <a-entity template="src: #platform9" data-num="2"></a-entity>
      <a-entity template="src: #platform10" data-num="1"></a-entity>
      <a-entity template="src: #platform11" data-num="3"></a-entity>
      <a-entity template="src: #platform12" data-num="3"></a-entity>
      <a-entity template="src: #platform13" data-num="4"></a-entity>
      <a-entity template="src: #platform15" data-num="2"></a-entity>
      <a-entity template="src: #platform16" data-num="3"></a-entity>
      <a-entity template="src: #platform16B" data-num="3"></a-entity>
    </a-entity>

    <a-entity position="40 13 100">
      <a-entity template="src: #platform9" data-num="2"></a-entity>
      <a-entity template="src: #platform10" data-num="1"></a-entity>
      <a-entity template="src: #platform11" data-num="3"></a-entity>
      <a-entity template="src: #platform12" data-num="3"></a-entity>
      <a-entity template="src: #platform13" data-num="4"></a-entity>
      <a-entity template="src: #platform15" data-num="2"></a-entity>
      <a-entity template="src: #platform16" data-num="3"></a-entity>
      <a-entity template="src: #platform16B" data-num="3"></a-entity>
    </a-entity>
<!-- FIN TEST -->

<!--  -->

    <a-entity position="-50 0 -50">
      <a-entity template="src: #platform9" data-num="2"></a-entity>
      <a-entity template="src: #platform10" data-num="1"></a-entity>
      <a-entity template="src: #platform11" data-num="3"></a-entity>
      <a-entity template="src: #platform12" data-num="3"></a-entity>
      <a-entity template="src: #platform13" data-num="4"></a-entity>
      <a-entity template="src: #platform15" data-num="2"></a-entity>
      <a-entity template="src: #platform16" data-num="3"></a-entity>
      <a-entity template="src: #platform16B" data-num="3"></a-entity>
    </a-entity>

    <a-entity position="40 13 100">
      <a-entity template="src: #platform9" data-num="2"></a-entity>
      <a-entity template="src: #platform10" data-num="1"></a-entity>
      <a-entity template="src: #platform11" data-num="3"></a-entity>
      <a-entity template="src: #platform12" data-num="3"></a-entity>
      <a-entity template="src: #platform13" data-num="4"></a-entity>
      <a-entity template="src: #platform15" data-num="2"></a-entity>
      <a-entity template="src: #platform16" data-num="3"></a-entity>
      <a-entity template="src: #platform16B" data-num="3"></a-entity>
    </a-entity>

    <!-- TEST -->

    <a-entity position="50 20 100">
      <a-entity template="src: #platform9" data-num="2"></a-entity>
      <a-entity template="src: #platform10" data-num="1"></a-entity>
      <a-entity template="src: #platform11" data-num="3"></a-entity>
      <a-entity template="src: #platform12" data-num="3"></a-entity>
      <a-entity template="src: #platform13" data-num="4"></a-entity>
      <a-entity template="src: #platform15" data-num="2"></a-entity>
      <a-entity template="src: #platform16" data-num="3"></a-entity>
      <a-entity template="src: #platform16B" data-num="3"></a-entity>
    </a-entity>

    <a-entity position="40 13 100">
      <a-entity template="src: #platform9" data-num="2"></a-entity>
      <a-entity template="src: #platform10" data-num="1"></a-entity>
      <a-entity template="src: #platform11" data-num="3"></a-entity>
      <a-entity template="src: #platform12" data-num="3"></a-entity>
      <a-entity template="src: #platform13" data-num="4"></a-entity>
      <a-entity template="src: #platform15" data-num="2"></a-entity>
      <a-entity template="src: #platform16" data-num="3"></a-entity>
      <a-entity template="src: #platform16B" data-num="3"></a-entity>
    </a-entity>
<!-- FIN TEST -->

<!--  -->

    <a-entity position="40 0 100">
      <a-entity template="src: #platform9" data-num="2"></a-entity>
      <a-entity template="src: #platform10" data-num="1"></a-entity>
      <a-entity template="src: #platform11" data-num="3"></a-entity>
      <a-entity template="src: #platform12" data-num="3"></a-entity>
      <a-entity template="src: #platform13" data-num="4"></a-entity>
      <a-entity template="src: #platform15" data-num="2"></a-entity>
      <a-entity template="src: #platform16" data-num="3"></a-entity>
      <a-entity template="src: #platform16B" data-num="3"></a-entity>
    </a-entity>

    <a-entity position="40 13 100">
      <a-entity template="src: #platform9" data-num="2"></a-entity>
      <a-entity template="src: #platform10" data-num="1"></a-entity>
      <a-entity template="src: #platform11" data-num="3"></a-entity>
      <a-entity template="src: #platform12" data-num="3"></a-entity>
      <a-entity template="src: #platform13" data-num="4"></a-entity>
      <a-entity template="src: #platform15" data-num="2"></a-entity>
      <a-entity template="src: #platform16" data-num="3"></a-entity>
      <a-entity template="src: #platform16B" data-num="3"></a-entity>
    </a-entity>

    <!-- TEST -->

    <a-entity position="50 20 100">
      <a-entity template="src: #platform9" data-num="2"></a-entity>
      <a-entity template="src: #platform10" data-num="1"></a-entity>
      <a-entity template="src: #platform11" data-num="3"></a-entity>
      <a-entity template="src: #platform12" data-num="3"></a-entity>
      <a-entity template="src: #platform13" data-num="4"></a-entity>
      <a-entity template="src: #platform15" data-num="2"></a-entity>
      <a-entity template="src: #platform16" data-num="3"></a-entity>
      <a-entity template="src: #platform16B" data-num="3"></a-entity>
    </a-entity>

    <a-entity position="40 13 100">
      <a-entity template="src: #platform9" data-num="2"></a-entity>
      <a-entity template="src: #platform10" data-num="1"></a-entity>
      <a-entity template="src: #platform11" data-num="3"></a-entity>
      <a-entity template="src: #platform12" data-num="3"></a-entity>
      <a-entity template="src: #platform13" data-num="4"></a-entity>
      <a-entity template="src: #platform15" data-num="2"></a-entity>
      <a-entity template="src: #platform16" data-num="3"></a-entity>
      <a-entity template="src: #platform16B" data-num="3"></a-entity>
    </a-entity>
<!-- FIN TEST -->


<!--  -->

    <a-entity position="-10 0 -50">
      <a-entity template="src: #platform9" data-num="2"></a-entity>
      <a-entity template="src: #platform10" data-num="1"></a-entity>
      <a-entity template="src: #platform11" data-num="3"></a-entity>
      <a-entity template="src: #platform12" data-num="3"></a-entity>
      <a-entity template="src: #platform13" data-num="4"></a-entity>
      <a-entity template="src: #platform15" data-num="2"></a-entity>
      <a-entity template="src: #platform16" data-num="3"></a-entity>
      <a-entity template="src: #platform16B" data-num="3"></a-entity>
    </a-entity>

    <a-entity position="40 13 100">
      <a-entity template="src: #platform9" data-num="2"></a-entity>
      <a-entity template="src: #platform10" data-num="1"></a-entity>
      <a-entity template="src: #platform11" data-num="3"></a-entity>
      <a-entity template="src: #platform12" data-num="3"></a-entity>
      <a-entity template="src: #platform13" data-num="4"></a-entity>
      <a-entity template="src: #platform15" data-num="2"></a-entity>
      <a-entity template="src: #platform16" data-num="3"></a-entity>
      <a-entity template="src: #platform16B" data-num="3"></a-entity>
    </a-entity>

    <a-entity position="50 20 100">
      <a-entity template="src: #platform9" data-num="2"></a-entity>
      <a-entity template="src: #platform10" data-num="1"></a-entity>
      <a-entity template="src: #platform11" data-num="3"></a-entity>
      <a-entity template="src: #platform12" data-num="3"></a-entity>
      <a-entity template="src: #platform13" data-num="4"></a-entity>
      <a-entity template="src: #platform15" data-num="2"></a-entity>
      <a-entity template="src: #platform16" data-num="3"></a-entity>
      <a-entity template="src: #platform16B" data-num="3"></a-entity>
    </a-entity>

    <a-entity position="40 13 100">
      <a-entity template="src: #platform9" data-num="2"></a-entity>
      <a-entity template="src: #platform10" data-num="1"></a-entity>
      <a-entity template="src: #platform11" data-num="3"></a-entity>
      <a-entity template="src: #platform12" data-num="3"></a-entity>
      <a-entity template="src: #platform13" data-num="4"></a-entity>
      <a-entity template="src: #platform15" data-num="2"></a-entity>
      <a-entity template="src: #platform16" data-num="3"></a-entity>
      <a-entity template="src: #platform16B" data-num="3"></a-entity>
    </a-entity>
<!-- FIN TEST -->

<!--  -->

    <a-entity position="0 0 0">
      <a-entity template="src: #platform9" data-num="2"></a-entity>
      <a-entity template="src: #platform10" data-num="1"></a-entity>
      <a-entity template="src: #platform11" data-num="3"></a-entity>
      <a-entity template="src: #platform12" data-num="3"></a-entity>
      <a-entity template="src: #platform13" data-num="4"></a-entity>
      <a-entity template="src: #platform15" data-num="2"></a-entity>
      <a-entity template="src: #platform16" data-num="3"></a-entity>
      <a-entity template="src: #platform16B" data-num="3"></a-entity>
    </a-entity>

    <a-entity position="40 13 100">
      <a-entity template="src: #platform9" data-num="2"></a-entity>
      <a-entity template="src: #platform10" data-num="1"></a-entity>
      <a-entity template="src: #platform11" data-num="3"></a-entity>
      <a-entity template="src: #platform12" data-num="3"></a-entity>
      <a-entity template="src: #platform13" data-num="4"></a-entity>
      <a-entity template="src: #platform15" data-num="2"></a-entity>
      <a-entity template="src: #platform16" data-num="3"></a-entity>
      <a-entity template="src: #platform16B" data-num="3"></a-entity>
    </a-entity>

    <!-- TEST -->

    <a-entity position="50 20 100">
      <a-entity template="src: #platform9" data-num="2"></a-entity>
      <a-entity template="src: #platform10" data-num="1"></a-entity>
      <a-entity template="src: #platform11" data-num="3"></a-entity>
      <a-entity template="src: #platform12" data-num="3"></a-entity>
      <a-entity template="src: #platform13" data-num="4"></a-entity>
      <a-entity template="src: #platform15" data-num="2"></a-entity>
      <a-entity template="src: #platform16" data-num="3"></a-entity>
      <a-entity template="src: #platform16B" data-num="3"></a-entity>
    </a-entity>

    <a-entity position="40 13 100">
      <a-entity template="src: #platform9" data-num="2"></a-entity>
      <a-entity template="src: #platform10" data-num="1"></a-entity>
      <a-entity template="src: #platform11" data-num="3"></a-entity>
      <a-entity template="src: #platform12" data-num="3"></a-entity>
      <a-entity template="src: #platform13" data-num="4"></a-entity>
      <a-entity template="src: #platform15" data-num="2"></a-entity>
      <a-entity template="src: #platform16" data-num="3"></a-entity>
      <a-entity template="src: #platform16B" data-num="3"></a-entity>
    </a-entity>
<!-- FIN TEST -->


<!-- TEST -->

    <a-entity position="-60 0 0"  rotation="0 45 0">
      <a-entity template="src: #platform9" data-num="2"></a-entity>
      <a-entity template="src: #platform10" data-num="1"></a-entity>
      <a-entity template="src: #platform11" data-num="3"></a-entity>
      <a-entity template="src: #platform12" data-num="3"></a-entity>
      <a-entity template="src: #platform13" data-num="4"></a-entity>
      <a-entity template="src: #platform15" data-num="2"></a-entity>
      <a-entity template="src: #platform16" data-num="3"></a-entity>
      <a-entity template="src: #platform16B" data-num="3"></a-entity>
    </a-entity>

    <a-entity position="40 13 100">
      <a-entity template="src: #platform9" data-num="2"></a-entity>
      <a-entity template="src: #platform10" data-num="1"></a-entity>
      <a-entity template="src: #platform11" data-num="3"></a-entity>
      <a-entity template="src: #platform12" data-num="3"></a-entity>
      <a-entity template="src: #platform13" data-num="4"></a-entity>
      <a-entity template="src: #platform15" data-num="2"></a-entity>
      <a-entity template="src: #platform16" data-num="3"></a-entity>
      <a-entity template="src: #platform16B" data-num="3"></a-entity>
    </a-entity>

    <a-entity position="50 20 100">
      <a-entity template="src: #platform9" data-num="2"></a-entity>
      <a-entity template="src: #platform10" data-num="1"></a-entity>
      <a-entity template="src: #platform11" data-num="3"></a-entity>
      <a-entity template="src: #platform12" data-num="3"></a-entity>
      <a-entity template="src: #platform13" data-num="4"></a-entity>
      <a-entity template="src: #platform15" data-num="2"></a-entity>
      <a-entity template="src: #platform16" data-num="3"></a-entity>
      <a-entity template="src: #platform16B" data-num="3"></a-entity>
    </a-entity>

    <a-entity position="40 13 100">
      <a-entity template="src: #platform9" data-num="2"></a-entity>
      <a-entity template="src: #platform10" data-num="1"></a-entity>
      <a-entity template="src: #platform11" data-num="3"></a-entity>
      <a-entity template="src: #platform12" data-num="3"></a-entity>
      <a-entity template="src: #platform13" data-num="4"></a-entity>
      <a-entity template="src: #platform15" data-num="2"></a-entity>
      <a-entity template="src: #platform16" data-num="3"></a-entity>
      <a-entity template="src: #platform16B" data-num="3"></a-entity>
    </a-entity>
<!-- FIN FOND -->
    <a-entity position="-10 0 40"  rotation="0 45 0">
      <a-entity template="src: #platform9" data-num="2"></a-entity>
      <a-entity template="src: #platform10" data-num="1"></a-entity>
      <a-entity template="src: #platform11" data-num="3"></a-entity>
      <a-entity template="src: #platform12" data-num="3"></a-entity>
      <a-entity template="src: #platform13" data-num="4"></a-entity>
      <a-entity template="src: #platform15" data-num="2"></a-entity>
      <a-entity template="src: #platform16" data-num="3"></a-entity>
      <a-entity template="src: #platform16B" data-num="3"></a-entity>
    </a-entity>

    <a-entity position="150 50 100">
      <a-entity template="src: #platform9" data-num="2"></a-entity>
      <a-entity template="src: #platform10" data-num="1"></a-entity>
      <a-entity template="src: #platform11" data-num="3"></a-entity>
      <a-entity template="src: #platform12" data-num="3"></a-entity>
      <a-entity template="src: #platform13" data-num="4"></a-entity>
      <a-entity template="src: #platform14" data-num="16"></a-entity>
      <a-entity template="src: #platform15" data-num="2"></a-entity>
      <a-entity template="src: #platform16" data-num="3"></a-entity>
      <a-entity template="src: #platform16B" data-num="3"></a-entity>
    </a-entity>

    <a-entity position="-40 15 -60">
      <a-entity template="src: #platform9" data-num="2"></a-entity>
      <a-entity template="src: #platform10" data-num="1"></a-entity>
      <a-entity template="src: #platform11" data-num="3"></a-entity>
      <a-entity template="src: #platform12" data-num="3"></a-entity>
      <a-entity template="src: #platform13" data-num="4"></a-entity>
      <a-entity template="src: #platform15" data-num="2"></a-entity>
      <a-entity template="src: #platform16" data-num="3"></a-entity>
      <a-entity template="src: #platform16B" data-num="3"></a-entity>
    </a-entity>

    <a-entity position="-60 15 -20">
      <a-entity template="src: #platform9" data-num="2"></a-entity>
      <a-entity template="src: #platform10" data-num="1"></a-entity>
      <a-entity template="src: #platform11" data-num="3"></a-entity>
      <a-entity template="src: #platform12" data-num="3"></a-entity>
      <a-entity template="src: #platform13" data-num="4"></a-entity>
      <a-entity template="src: #platform15" data-num="2"></a-entity>
      <a-entity template="src: #platform16" data-num="3"></a-entity>
      <a-entity template="src: #platform16B" data-num="3"></a-entity>
    </a-entity>

    <a-entity position="-70 0 -30">
      <a-entity template="src: #platform9" data-num="2"></a-entity>
      <a-entity template="src: #platform10" data-num="1"></a-entity>
      <a-entity template="src: #platform11" data-num="3"></a-entity>
      <a-entity template="src: #platform12" data-num="3"></a-entity>
      <a-entity template="src: #platform13" data-num="4"></a-entity>
      <a-entity template="src: #platform15" data-num="2"></a-entity>
      <a-entity template="src: #platform16" data-num="3"></a-entity>
      <a-entity template="src: #platform16B" data-num="3"></a-entity>
    </a-entity>



<!-- FIN FOND -->
    <a-entity position="40 13 100">
      <a-entity template="src: #platform9" data-num="2"></a-entity>
      <a-entity template="src: #platform10" data-num="1"></a-entity>
      <a-entity template="src: #platform11" data-num="3"></a-entity>
      <a-entity template="src: #platform12" data-num="3"></a-entity>
      <a-entity template="src: #platform13" data-num="4"></a-entity>
      <a-entity template="src: #platform15" data-num="2"></a-entity>
      <a-entity template="src: #platform16" data-num="3"></a-entity>
      <a-entity template="src: #platform16B" data-num="3"></a-entity>
    </a-entity>

    <a-entity position="50 20 100">
      <a-entity template="src: #platform9" data-num="2"></a-entity>
      <a-entity template="src: #platform10" data-num="1"></a-entity>
      <a-entity template="src: #platform11" data-num="3"></a-entity>
      <a-entity template="src: #platform12" data-num="3"></a-entity>
      <a-entity template="src: #platform13" data-num="4"></a-entity>
      <a-entity template="src: #platform15" data-num="2"></a-entity>
      <a-entity template="src: #platform16" data-num="3"></a-entity>
      <a-entity template="src: #platform16B" data-num="3"></a-entity>
    </a-entity>

    <a-entity position="40 13 100">
      <a-entity template="src: #platform9" data-num="2"></a-entity>
      <a-entity template="src: #platform10" data-num="1"></a-entity>
      <a-entity template="src: #platform11" data-num="3"></a-entity>
      <a-entity template="src: #platform12" data-num="3"></a-entity>
      <a-entity template="src: #platform13" data-num="4"></a-entity>
      <a-entity template="src: #platform15" data-num="2"></a-entity>
      <a-entity template="src: #platform16" data-num="3"></a-entity>
      <a-entity template="src: #platform16B" data-num="3"></a-entity>
    </a-entity>
<!-- FIN TEST -->


<a-entity position="-80 0 0" rotation="0 45 0">


    <a-entity position="40 0 100">
      <a-entity template="src: #platform9" data-num="2"></a-entity>
      <a-entity template="src: #platform10" data-num="1"></a-entity>
      <a-entity template="src: #platform11" data-num="3"></a-entity>
      <a-entity template="src: #platform12" data-num="3"></a-entity>
      <a-entity template="src: #platform13" data-num="4"></a-entity>
      <a-entity template="src: #platform15" data-num="2"></a-entity>
      <a-entity template="src: #platform16" data-num="3"></a-entity>
      <a-entity template="src: #platform16B" data-num="3"></a-entity>
    </a-entity>

    <a-entity position="40 13 100">
      <a-entity template="src: #platform9" data-num="2"></a-entity>
      <a-entity template="src: #platform10" data-num="1"></a-entity>
      <a-entity template="src: #platform11" data-num="3"></a-entity>
      <a-entity template="src: #platform12" data-num="3"></a-entity>
      <a-entity template="src: #platform13" data-num="4"></a-entity>
      <a-entity template="src: #platform15" data-num="2"></a-entity>
      <a-entity template="src: #platform16" data-num="3"></a-entity>
      <a-entity template="src: #platform16B" data-num="3"></a-entity>
    </a-entity>

    <!-- TEST -->

    <a-entity position="50 20 100">
      <a-entity template="src: #platform9" data-num="2"></a-entity>
      <a-entity template="src: #platform10" data-num="1"></a-entity>
      <a-entity template="src: #platform11" data-num="3"></a-entity>
      <a-entity template="src: #platform12" data-num="3"></a-entity>
      <a-entity template="src: #platform13" data-num="4"></a-entity>
      <a-entity template="src: #platform15" data-num="2"></a-entity>
      <a-entity template="src: #platform16" data-num="3"></a-entity>
      <a-entity template="src: #platform16B" data-num="3"></a-entity>
    </a-entity>

    <a-entity position="40 13 100">
      <a-entity template="src: #platform9" data-num="2"></a-entity>
      <a-entity template="src: #platform10" data-num="1"></a-entity>
      <a-entity template="src: #platform11" data-num="3"></a-entity>
      <a-entity template="src: #platform12" data-num="3"></a-entity>
      <a-entity template="src: #platform13" data-num="4"></a-entity>
      <a-entity template="src: #platform15" data-num="2"></a-entity>
      <a-entity template="src: #platform16" data-num="3"></a-entity>
      <a-entity template="src: #platform16B" data-num="3"></a-entity>
    </a-entity>
</a-entity>
<!-- FIN TEST -->


<a-entity position="50 0 50">
  <a-entity template="src: #platform9" data-num="2"></a-entity>
  <a-entity template="src: #platform10" data-num="1"></a-entity>
  <a-entity template="src: #platform11" data-num="3"></a-entity>
  <a-entity template="src: #platform12" data-num="3"></a-entity>
  <a-entity template="src: #platform13" data-num="4"></a-entity>
  <a-entity template="src: #platform15" data-num="2"></a-entity>
  <a-entity template="src: #platform16" data-num="3"></a-entity>
  <a-entity template="src: #platform16B" data-num="3"></a-entity>
</a-entity>

<a-entity position="50 13 50">
  <a-entity template="src: #platform9" data-num="2"></a-entity>
  <a-entity template="src: #platform10" data-num="1"></a-entity>
  <a-entity template="src: #platform11" data-num="3"></a-entity>
  <a-entity template="src: #platform12" data-num="3"></a-entity>
  <a-entity template="src: #platform13" data-num="4"></a-entity>
  <a-entity template="src: #platform15" data-num="2"></a-entity>
  <a-entity template="src: #platform16" data-num="3"></a-entity>
  <a-entity template="src: #platform16B" data-num="3"></a-entity>
</a-entity>

<a-entity position="50 13 50">
  <a-entity template="src: #platform9" data-num="2"></a-entity>
  <a-entity template="src: #platform10" data-num="1"></a-entity>
  <a-entity template="src: #platform11" data-num="3"></a-entity>
  <a-entity template="src: #platform12" data-num="3"></a-entity>
  <a-entity template="src: #platform13" data-num="4"></a-entity>
  <a-entity template="src: #platform15" data-num="2"></a-entity>
  <a-entity template="src: #platform16" data-num="3"></a-entity>
  <a-entity template="src: #platform16B" data-num="3"></a-entity>
</a-entity>

<a-entity position="-40 0 0">
  <a-entity template="src: #platform17" data-num="1"></a-entity>
  <a-entity template="src: #platform18" data-num="1"></a-entity>
  <a-entity template="src: #platform19" data-num="3"></a-entity>
  <a-entity template="src: #platform20" data-num="2"></a-entity>
  <a-entity template="src: #platform21" data-num="3"></a-entity>
  <a-entity template="src: #platform22" data-num="1"></a-entity>
  <a-entity template="src: #platform23" data-num="2"></a-entity>
  <a-entity template="src: #platform24" data-num="3"></a-entity>
</a-entity>
          <a-entity geometry="primitive: cylinder; radius: 2; segmentsRadial: 6; openEnded: false; thetaLength: 360; height: 0.2;" position="0 0 -29.8"
                  material="side: double; color: #DD2C00"></a-entity>

  <a-sky color="#252243"></a-sky>
</a-scene>







    </body>
</html>
