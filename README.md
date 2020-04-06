# Ernst - Extendable Robust Native-like Standard Components

[Jump to usage](#Get-your-hands-dirty-and-see-for-yourself)

## Time to spring-clean your frontend?

Are you stuck with five different frontend frameworks and every one uses its own set of UI components? Do you have an old web application that could need some quality of life improvements, but can't afford a complete rewrite? Are you using mostly HTML5 for your project and not to keen on bloating down on javascript just to get a single robust component that is being actively maintained? Do you just wish you could get a normalized date picker across all browsers? Then you're in luck, for we have hopefully the right solution for you!


## Accessibility first and built to be extendable

In order to spring-clean, you will need the right tools for it. Ernst offers components that puts accessibility first, giving your users a solid and robust experience at the lowest level so that you can put your main effort into improving the experience on a higher level. It might also be that you want to customize the components and tailor them to your own need. No worries, the components are built so you can easily make your changes at source code level. You can also extend and derive from these components. That way, you keep both the original component and have a new custom enhanced component. All components are also highly stylable, getting you the look you actually want.

## Ease of use, legacy support and no third party dependencies besides browser polyfills
The web is an enormous place and the surrounding context for each project is broad and unique. By making these components as easy to use as possible and straight to the point, we hope to fill the gap where other solutions don't feel satisfactory. Ernst also strives to support legacy, which in theory could go back as far as IE8 with the right amounts of polyfills. 

## Close adherence to web standards
Many components will be direct implementations of HTML standard or WAI-ARIA authoring practices. This is to ensure that they can in fact as a drop-in replacement and so you can expect them to behave as standard HTML elements. This will also be the reason why the scope of each component will be limited. They aim to solve the most basic and universal needs for everyone. If that is not quite enough, then that's where the extendable part comes into play. You can always use the components as basis to add the final missing piece you need for your project.


## Get your hands dirty and see for yourself

*(Whoops, we don't have any good way on how to use the components yet, stay tuned for that!)*

Take a look into the our collection of components and see how they can help you with your project!

### Animation

CSS transitions and animations has it limits, these will help you with some common problems that you might encounter. Or maybe just make life a bit easier during development.

* `<animation-height/>`

### Input

Normlized, accessible inputs with proper styling and custom content, finally!

* `<input-color/>`
* `<input-date/>`
* `<input-select/>`
* `<input-tree/>`

### Layout

Layout is not always a pure CSS problem. Sometimes you need some scripting to help you out, other times there are a great number of accessibility concerns that needs to be addressed.

* `<layout-modal/>`
* `<layout-sticky/>`


## FAQ

> Aren't there already many similar projects?

Yes, for example [Elix](https://component.kitchen/elix) which has the same driving philosophy. However in their case, they are building it around Web Components and Evergreen browsers. Ernst focuses on Custom Elements only in order to support legacy browsers as much as possible. Legacy browser support is still a large factor for many applications, and Ernst intends to serve as a drop-in replacement for any current solutions out there, so high compatibility is a key factor.

> Why are you using the old deprecated V0 version of Custom Elements?

Similar to the previous answer, the main focus of Ernst is to bring all current web sites and applications out there up to speed with accessible and robust core components. By lowering the entry level to use the components, a faster adoption rate can hopefully be achieved and increase the general level of accessibility on the web. Older browser will be polyfilled regardless to support Custom Elements, and the V0 API is based on ES5, compared to V1 which is based around ES6 classes. The consequences is that V1 usage will require higher effort to ensure the native V1 API still works while still transpiling the code to ES5. Another aspect is that when all browser use the same polyfill instead of mixing with native code, is that you can rely more safely on components behaving the same across browsers.

> But that's what build tools are for, so you don't have to think about that stuff!

True, but not all projects have build tools setup for their websites and applications. By adding that as a requirement, the entry level will increase and thus slowing down the adoption rate. The end goal is to raise the general web experience and increase accessibility as much as possible.

> How will you handle migration and breaking changes?

Custom Elements poses the same challenges as native Html5 elements, which is the ubiquitous nature of them. Once in place and used, it will become harder and harder to refactor. If you are not in 100% control of your content, there may be implicit hard dependencies on the singleton nature of the custom elements. This is another reason for why the scope of each element will be quite small and constrained, and focus more on enable the implementations than offer a complete full implementations of every possible cases. It is in the same manner as [The Extensible Web Manifesto](https://extensiblewebmanifesto.org/), provide a foundation to build upon. There will however be breaking changes regardless (nothing is perfect out-of-the-box), so thats is why each element are made in isolation of each other, and can easily be extended or renamed. More to come about this, but be assured that this is always an active issue that Ernst will be aware of.

> Is anyone using these components in production yet?

Yes, [Stratsys](https://www.stratsys.com/) where these components were originally incepted, uses them across a wide assortment of product suites which are used by a big part of Swedens public sector.


> Wait up a minute, isn't the name Ernst and all this talk about spring-cleaning suspiciously similar to Swedens most wholesome home renovator, [Ernst Kirchsteiger](https://www.google.se/search?q=ernst+kirchsteiger+sommar+med+ernst&tbm=isch)? 

Maybe.