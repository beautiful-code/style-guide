## Javascript Style Guide

### Import Guidelines

Imports should be grouped as following with an empty line in between.

- Third party imports with react and react-redux packages at the top.
- UI related imports with 'common components', 'page components' and scss at the top
- Other imports (ex: ****'reducers.js', 'actionCreators.js', 'helpers.js')

-----

### React Component Methods Order

Methods in a react class component should be of the following order.

1. static methods and properties
2. lifecycle methods: `displayName`, `propTypes`, `contextTypes`, `childContextTypes`, `mixins`, `statics`, `defaultProps`, `constructor`, `getDefaultProps`, `state`, `getInitialState`, `getChildContext`, `getDerivedStateFromProps`, `componentWillMount`, `UNSAFE_componentWillMount`, `componentDidMount`, `componentWillReceiveProps`, `UNSAFE_componentWillReceiveProps`, `shouldComponentUpdate`, `componentWillUpdate`, `UNSAFE_componentWillUpdate`, `getSnapshotBeforeUpdate`, `componentDidUpdate`, `componentDidCatch`, `componentWillUnmount` (in this order).
3. custom methods and event handlers
4. `render` method

Eslint plugin: [react/sort-comp](https://github.com/yannickcr/eslint-plugin-react/blob/master/docs/rules/sort-comp.md).

-----

### Event handler functions naming convention

Functions name should start with `handle`. Followed by what the event does (noun). Should end with what type of event it is (verb)

Ex: `handleFormSubmit` , `handleModalOk`, `handleModalClose`, `handleModalCancel`, `handleDownloadClick`

-----

### Where should CSS go?

CSS goes in three places- main-styles.scss, beside a Generic component and root scss file at each domain level

-----

### Redux action name convention

To avoid bugs caused by conflicts in redux action names, suffix with every action name it's domain name.

Ex: `OPEN_FILTER_DROPDOWN_IN_HOME` where `IN_HOME` is the suffix to identify the domain.

-----
