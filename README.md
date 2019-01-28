# Gatsby + Jest template

1. Install all your dependencies.

Using npm
```bash
$ npm install 
```

Using yarn
```bash
$ yarn 
```

2. Then you can add some test to the test path:Test folder is in `/src/components/__test__`

Test example
```javascript
import React from 'react';
import renderer from 'react-test-renderer';

import Header from '../header';

describe('Header', () => {
	it('renders correctly', () => {
		const tree = renderer.create(<Header siteTitle="Default Starter" />).toJSON();
		expect(tree).toMatchSnapshot();
	});
});

```

3. To run your test

Using npm
```bash
$ npm run test
```

Using yarn
```bash
$ yarn test
```