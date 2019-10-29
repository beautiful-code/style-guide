## Javascript Style Guide


### Import Guidelines
Imports should be grouped as following with an empty line in between
- Third party imports with react and react-redux packages at the top.
- UI related imports with 'common components', 'page components' and scss at the top
- Other imports (ex: ****'reducers.js', 'actionCreators.js', 'helpers.js')

-----

### React Component Methods Order
Methods in a react class component should be of the following order
- static propTypes
- static defaultProps
- state
- getDerivedStateFromProps
- componentDidMount
- componentWillUnmount
- componentDidUpdate
- shouldComponentUpdate
- Other methods (event handler functions)
- render

-----
### Event handler functions naming convention
Functions name should start with `handle`. Followed by what the event does (noun). Should end with what type of event it is (verb)

Ex: `handleFormSubmit` , `handleModalOk`, `handleModalClose`, `handleModalCancel`, `handleDownloadClick`

-----

### Where should CSS go?
CSS goes in three places- main-styles.scss, beside a Generic component and root scss file at each domain level


-----