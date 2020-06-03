## [awesome-angular](https://github.com/PatrickJS/awesome-angular)

## angular article link
  - https://indepth.dev/
  - https://angular.io/resources?category=community

## Angular Life Cycle:
  - https://www.freecodecamp.org/news/the-best-angular-examples/
  - https://www.freecodecamp.org/news/angular-lifecycle-hooks/
  - https://angular.io/guide/lifecycle-hooks
  
## Bundle size

  - https://medium.com/angular-in-depth/optimize-angular-bundle-size-in-4-steps-4a3b3737bf45
 -  https://www.npmjs.com/package/source-map-explorer
  - npm package "Gzipper" : https://www.npmjs.com/package/gzipper
  - how angular bundles: https://www.freecodecamp.org/news/how-to-configure-webpack-4-with-angular-7-a-complete-guide-9a23c879f471/
  
  
## loading spinner
 - https://christianlydemann.com/four-ways-to-create-loading-spinners-in-an-angular-app/
 
## GlobalErrorHandler ==> error handling
  - https://medium.com/angular-in-depth/expecting-the-unexpected-best-practices-for-error-handling-in-angular-21c3662ef9e4
  
## HttpInterceptor
  - https://medium.com/angular-in-depth/top-10-ways-to-use-interceptors-in-angular-db450f8a62d6
  - https://angular.io/guide/http

## ViewChild
```
<p #pRef>
Start editing to see some magic happen :)
</p>

@ViewChild(HelloComponent, {static: false}) hello: HelloComponent;
@ViewChild('pRef', {static: false}) pRef: ElementRef;

  ngAfterViewInit() {
    console.log('Hello ', this.hello.name); 
	this.pRef.nativeElement.innerHTML = "DOM updated successfully!!!";
  }
```

## ViewChildren
```
<hello  name="Angular 6"  ></hello>
<hello  name="Angular 7"  ></hello>
<hello  name="Angular 8"  ></hello>

 @ViewChildren(HelloComponent) hellos: QueryList<any>;
  
  ngAfterViewInit() {
     this.hellos.forEach(hello => console.log(hello));
  }
 ```

## Various Packages & their usage
- [awesome path](https://github.com/sindresorhus/awesome)
- [awesome angular packages](https://github.com/PatrickJS/awesome-angular#third-party-components) 
- subsink - library to collection subscibeption and unsubscribe using single method call in  onDestroy()