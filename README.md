# Export the mongodb collection to csv or json

## Usage
```bash
 $ npm install mongotojson --save
```
```javascript
var convert = require('mongotojson');
var options = {
	database: 'product', // required
	collection: 'users', // required
	fields: ['name','address'], // optional
	output: './output/users.csv or .json', // required
};
convert.export(options, function (err, success) {
	console.log(err);
	console.log(success);
});
``
