# Flask-Angular

Change "$interpolateProvider", because confrict jinja2 markup.

    var app = angular.module('myapp', []);

    app.config(function($interpolateProvider) {
      $interpolateProvider.startSymbol('[[');
      $interpolateProvider.endSymbol(']]');
    });
    
