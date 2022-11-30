# NOTES

## REACT

* React is declarative and in charge of taking our declared code and performing all of the JavaScript/DOM steps to get us to our desired result.

* Component that rendered same way with same props can be wrapped with React.memo higher order component.

* Babel takes JSX and turn it to createElement.

* React.lazy function lets you render a dynamic import as a regular component and handles code-splitting.

* `<Suspense>` component with fallback could be used show spinner or loading state.

  ```
  <Suspense fallback={<div>Loading...</div>}>
    <OtherComponent />
  </Suspense>
  ```

* useLayoutEffect runs before useEffect to show something until.

* React.PureComponent is used for shouldComponentUpdate() hook.

* Loader is used in webpack to pre-process files.

* Virtual DOM is kept in memory and representation of real DOM. It is used to increase performance.

* All react components must act like pure function that takes props as arguments.

* In JSX, lowercase names are considered as HTML tag, so React components' name must be PascalCase.

* setState is asynchronous and might result in out of sync values. So, it is a good idea to pass a function to setState instead of an object.

* useEffect with no dependency invokes only when component mount.

* `<a>` tag triggers full page reload unlike routers `<Link>` component.

* ReactDOM.createPortal(child,container)

  child : React child can be rendered.

  container : DOM element exists outside of parent component.

* Reconciliation : The Virtual DOM (V-DOM) is an in-memory representation of Real DOM. The representation of a UI is kept in memory and synced with the "real" DOM. It's a step that happens between the render function being called and the displaying of elements on the screen. This entire process is called reconciliation. Simply, it is the process of deciding whether an update is necessary.

* React.ref is used for directly accession to a DOM node.

* useCallback is a hook used to prevent a function from being recreated on every component render.

* Flux helps react for keeping their data uni-directional. It is used for state management, like Redux.

* JSX gets transpiled to a React.createElement() function tree

  ```
  const Button = ({ onLogin }) => React.createElement(
  'div',
  { id: 'login-btn', onClick: onLogin },
  'Login'
  )
  ```

* Error Boundaries must be used as class component.

* State & Props : Props get passed to the component similar to function parameters whereas state is managed within the component similar to variables declared within a function.

* JavaScript is an interpreted language, not a compiled language. JavaScript is interpreted at runtime by the client browser.

* The Virtual DOM works in three simple steps.

  * Whenever any underlying data changes, the entire UI is re-rendered in Virtual DOM representation.
  * Then the difference between the previous DOM representation and the new one is calculated.
  * Once the calculations are done, the real DOM will be updated with only the things that have actually changed.
<br>
<br>

* The Shadow DOM is a browser technology designed primarily for scoping variables and CSS in web components. The Virtual DOM is a concept implemented by libraries in JavaScript on top of browser APIs.

* React Fiber is the new reconciliation engine or re-implementation of core algorithm in React v16. The goal of React Fiber is to increase its suitability for areas like animation, layout, gestures, ability to pause, abort, or reuse work and assign priority to different types of updates; and new concurrency primitives. Its headline feature is incremental rendering: the ability to split rendering work into chunks and spread it out over multiple frames.

* JavaScript engine is a software component that executes JavaScript code. All modern browsers have their own version.

  * V8 – Open-source JavaScript Engine developed by Google for Chrome
  * SpiderMonkey – The JavaScript Engine powering Mozilla Firefox
  * JavaScriptCore – Open-source JavaScript Engine developed by Apple for Safari
  * Chakra – A JavaScript Engine for Microsoft Edge
  * JerryScript – A JavaScript engine for the Internet of Things (Iot).
<br>
<br>

* 