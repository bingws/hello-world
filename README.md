# hello-world
arcgis api for JavaScript（NO.1 Initial map）
<!DOCTYPE html>
<html>
  <head>
    <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
    <meta name="viewport" content="initial-scale=1, maximum-scale=1,user-scalable=no"/>
    <title>Simple Map</title>
    //Esri本地样式加载
    <link rel="stylesheet" href="http://localhost/arcgis_js_api/library/3.17/3.17/esri/css/esri.css">
    <style>
      html, body, #map {
        height: 100%;
        margin: 0;
        padding: 0;
      }
    </style>
   //初始化所需的API
    <script src="http://localhost/arcgis_js_api/library/3.17/3.17/init.js"></script>
    <script>
        var map;

        require(["esri/map", "dojo/domReady!"], function (Map) {
            map = new Map("map", {
                basemap: "topo",  //For full list of pre-defined basemaps, navigate to http://arcg.is/1JVo6Wd
                center: [-122.45, 37.75], // longitude, latitude
                zoom: 13
            });
        });
    </script>
  </head>

  <body>
    <div id="map"></div>
  </body>
</html>
