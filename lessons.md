# Angular QuickStart


## step 1
install npm / node. 
create folder, add package.json file, and paste the content from angular. 
run npm install.

## step 2

create a subfolder, 'app', and create your first angular component. 
`mkdir app` create the component `app/app.component.ts` (mind the .ts extension)

We need at least one <b>root component</b>, named AppComponent.
Every component has basicly the same footprint
- one or more `import` statements. 
- A `@Component decorator` that tells angular what template to use and how to create the component. 
- A `Component class` that controlls appearance/logic/behaviour. 

Component is a 'decorator function' that takes a 'metadata object' as its argument. We apply the function, by prefixing the Component with an @ symbol, so that it invokes the metadata, just above the class definition. 

@Component is a decorator, that allows to associate 'metadata' with the component class. The metadate tells Angular ohw to create and use the component.


example:
```js
@Component({
    selector: 'my-app',
    template: '<h1>my first angualr app</h1>'
    })
```

In the above example, we have a @Component with MetaData that holds two properties, or 'fields'. First the selector, and second the template. 