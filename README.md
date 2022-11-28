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

* Reconciliation is process of deciding whether an update is necessary.

* React.ref is used for directly accession to a DOM node.

* useCallback is a hook used to prevent a function from being recreated on every component render.

* Flux helps react for keeping their data uni-directional. It is used for state management, like Redux.