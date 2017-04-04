# Ruby (Hashes) vs. JavaScript (Dictionaries): Study

Use your favorite search engine and the provided readings to research and
respond to the following questions.

In your responses, be sure to cite any relevant sources you consulted in your
search. We ask you to write responses in your own words in order to see how you
process what you've read. Please do not respond with direct quotes from source
material. Instead, digest what you've read and repeat it in your own voice.

## Required Readings
-   Ruby-Doc.org
    -   [Hash#[]](http://ruby-doc.org/core-2.3.1/Hash.html#method-i-5B-5D)
    -   [Hash#delete](http://ruby-doc.org/core-2.3.1/Hash.html#method-i-5B-5D)
-   [Ruby Programming / Syntax / Literals - Interpolation](https://en.wikibooks.org/wiki/Ruby_Programming/Syntax/Literals#Interpolation)
-   Mozilla Developer Network
    -   [Working with objects - (Deleting properties)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Working_with_Objects#Deleting_properties)
    -   [Object.keys()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/keys)
    -   [Template literals](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Template_literals)

## Recommended Readings

-   Ruby-Doc.org
    -   [Class: Hash](http://ruby-doc.org/core-2.3.1/Hash.html)
    -   [Class: Symbol](http://ruby-doc.org/core-2.3.1/Symbol.html)
-   Mozilla Developer Network
    -   [Object - JavaScript | MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)
    -   [Working with objects - JavaScript | MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Working_with_Objects)

## Creating a Hash in Ruby

Create a hash named `dale` in Ruby with the following key-value pairs.  The keys
should be symbols.

| Key | Value |
| --- | --- |
| family_name | 'gribble' |
| given-name | 'dale' |
| occupation | 'exterminator' |

```ruby
dale = {
  family_name: 'gribble',
  'given-name': 'dale',
  occupation: 'exterminator'
}
```

## Adding Hash Keys in Ruby
Add a key named `middle name` to `dale` with the string "Alvin" as the value.
Add another key, `hobbies`, to `dale` with an array as the value. The array
should contain two strings, "drinking beer" and "conspiracy theories".  The keys
should be symbols.

```ruby
dale[:'middle name'] = 'Alvin'
dale[:hobbies] = ['drinking beer', 'conspiracy theories']
```

## Removing Hash Keys in Ruby

Remove the `middle name` key from `dale`.

```ruby
dale.delete(:'middle name')
```

## Modifying Hash Values in Ruby

Modify `dale` so that the value of the key `family_name` is "Gribble" and the
value of the key `given-name` is "Dale".

```ruby
dale[:family_name] = 'Gribble'
dale[:'given-name'] = 'Dale'
```

## Ruby Hash Methods

Using Ruby's Hash methods, set a variable named `dale_keys` to `dale`'s keys.
Additionally, set a variable named `dale_values` to `dale`'s values.'

```ruby
dale_keys = dale.keys
dale_values = dale.values
```

## Accessing Hash Properties and Values

Using Hash methods and string interpolation in Ruby, create a string using
`dale` that equals "My name is Dale Gribble and I'm an exterminator that enjoys
conspiracy theories.".

```ruby
string = "My name is #{dale[:'given-name']} #{dale[:family_name]} and I'm an #{dale[:occupation]} that enjoys #{dale[:hobbies][1]}."
```

## Creating a Dictionary in JavaScript

Create a dictionary named `hank` in JavaScript with the following key-value
pairs.

| Key | Value |
| --- | --- |
| family_name | 'hill' |
| given-name | 'hank' |
| occupation | 'propane and propane accessories salesman' |

```javascript
const hank = {
  family_name: 'hill',
  'given-name': 'hank',
  occupation: 'propane and propane accessories salesman'
}
```

## Adding Dictionary Properties in JavaScript

Add a property named `middle name` to `hank` with the string "Rutherford" as the
value.  Add another property, `hobbies`, to `hank` with an array as the value.
The array should contain two strings, "drinking beer" and "propane and propane
accessories".

```javascript
hank['middle name'] = 'Rutherford';
hank.hobbies = ['drinking beer', 'propane and propane accessories'];
```

## Removing Dictionary Properties in JavaScript

Remove the `middle name` property from `hank`.

```javascript
delete hank['middle name'];
```

## Modifying Dictionary Values in JavaScript

Modify `hank` so that the value of the key `family_name` is "Hill" and the value
of the key `given-name` is "Hank".

```javascript
hank.family_name = 'Hill';
hank['given-name'] = 'Hank';
```

## JavaScript Dictionary Methods

Using JavaScript's Array methods, set a variable named `hankKeys` to `hank`'s
keys.  Additionally, set a variable named `hankValues` to `hanks`'s values.'

```javascript
const hankKeys = Object.keys(hank);
const hankValues = Object.values(hank);
```

## Accessing Dictionary Properties and Values

Using dictionary methods and template literals in JavaScript, create a string
using `hank` that equals "My name is Hank Hill and I'm a propane and propane
accesories salesman that enjoys drinking beer.".

```javascript
const string = `My name is ${hank['given-name']} ${hank.family_name} and I'm a ${hank.occupation} that enjoys ${hank.hobbies[0]}.`;
```
