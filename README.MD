# ng-screenshot

--------------------------------------------------------------------------------

AngularJS directive for screenshot

A simple AngularJS directive for screenshot

# Examples:

--------------------------------------------------------------------------------

```html
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="utf-8">
  <title>ng-screenshot demo</title>
</head>

<body ng-app="demo" ng-controller="demoCtrl">
  <screenshot screenshot-trigger="#trigger">
    <h3>Here will be shot</h3>
    <span>{{name}}</span>
  </screenshot>
  <h3>Here will not be shot</h3>
  <button id="trigger" type="button" name="button">Screenshot</button>

  <screenshot screenshot-trigger="#trigger2">
    <h3>Here will be shot</h3>
    <span>{{email}}</span>
  </screenshot>
  <button id="trigger2" type="button" name="button">Screenshot</button>

  <script src="../node_modules/jquery/dist/jquery.min.js" charset="utf-8"></script>
  <script src="../node_modules/angular/angular.js" charset="utf-8"></script>
  <script src="../node_modules/html2canvas/dist/html2canvas.js" charset="utf-8"></script>
  <script src="../node_modules/file-saver/FileSaver.js" charset="utf-8"></script>
  <script src="../ng-screenshot.js" charset="utf-8"></script>

  <script type="text/javascript">
    angular.module('demo', ['ng-screenshot'])
      .controller('demoCtrl', function($scope) {
        $scope.name = 'Liujialun';
        $scope.email = "jialun.liu@hirain.com";
      })
  </script>
</body>

</html>
```

# Versions

--------------------------------------------------------------------------------

## Version 0.1.1

Bug fix for multi screenshots exists could not shot correctly.

## Version 0.1.0

See examples
