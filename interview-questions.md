# General Knowledge Questions:

Please write your answers in the code blocks.

**NOTICE:** Some (but not all) questions may be easier to answer with code or pseudocode. As an example, all of these are an acceptable answer to the question "How do you iterate a variable in PHP?"

```
$number++;
```

```
num = num + 1
```

```
variable "num" now equals "num" + 1
```

-----------------------------------------------------------------------

## Section: PHP

1. How do you get information from a form that is submitted using the "get" method?

```
$_GET['name'];
```

2. What is the correct way to create a function in PHP?

```
function functionName() { code; }
```

3. Name a method to output an array?

```
print_r($array);
```

4. Which operator is used to check if two values are equal and of same data type?

```
===
```

5. Which superglobal variable holds information about headers, paths, and script locations?

```
$_SERVER
```

6. Explain how `static function` works in PHP class methods.

```
Class Test { static public function answer() { return "correct"; } }
echo Test::answer();
```


7. What is the commonly used library for database connections?

```
MYSQLi
```

8. What is the commonly used library for making requests?

```
cURL
```

9. What is PHP function strlen?

```
Returns the length of a string.
```


## Section: SQL

For the below questions, assume you are using this table (named `Persons`):

| Id | FirstName | LastName  |
|----|-----------|-----------|
| 1  | Peter     | Jackson   |
| 2  | Adam      | Savage    |
| 3  | Linus     | Sebastian |
| 4  | Brent     | Spiner    |
| 5  | Doom      | Guy       |

1. How would you select just the first record and only the column `FirstName`?

```
SELECT FirstName FROM Persons LIMIT 1;
```

2. How would you select all the records where the `FirstName` is "Peter" and the `LastName` is "Jackson"?

```
SELECT * FROM Persons WHERE FirstName='Peter' AND LastName='Jackson';
```

3. How would you select all the records where the `LastName` starts with an "s"?

```
SELECT * FROM Persons WHERE LIKE 's%';
```

4. How would you select all the records where the `FirstName` is alphabetically between "Brent" and "Linus"?

```
SELECT * FROM Persons
WHERE FirstName BETWEEN "Brent" AND "Linus";
```

5. How would you insert the name "David Tennant"?

```
INSERT INTO Persons (FirstName, LastName) VALUES ('David', 'Tennant');
```

6. How would you change all the records where the `FirstName` is equal to "Peter" into "Samuel"?

```
UPDATE Persons
SET FirstName = "Samuel"
WHERE FirstName = "Peter"; 
```

7. How would you delete the records where the `LastName` is "Sebastian"?

```
DELETE FROM Persons WHERE LastName = "Sebastian";
```

8. How would you get the number of records in the `Persons` table?

```
SELECT COUNT(*) FROM Persons;
```

9. Give an example of how would you join 2 related tables together?

```
SELECT columns
FROM table1 JOIN table2 
ON column1 = column2
WHERE condition
```


## Section: Vanilla Javascript

1. How do you create a function in JavaScript?

```
function(variables) { code; }
```

2. How do you call a function named "myFunction"?

```
myFunction();
```

4. How to write an IF statement for executing some code if "i" is NOT equal to 5?

```
if (i != 5) {
  some code;
} 
```

5. How does a WHILE loop start?

```
while (condition) {
  code;
}
```

6. How does a FOR loop start?

```
for (condition) {
  code;
}
```

7. How do you round the number 7.25, to the nearest integer?

```
Math.round(7.25);
```

8. What will the following code return: Boolean(10 > 9)

```
true
```

## Section: jQuery

1. Can jQuery animate() method can be used to animate ANY CSS property?

```
No, only properties with a numeric value.
```

2. Which jQuery method is used to hide selected elements?

```
hide()
```

3. Which jQuery method is used to perform an asynchronous HTTP request?

```
ajax()
```

4. Look at the following selector: $("div p"). What does it select?

```
All <p> descendants of a <div>.
```


## Section: React

1. What is JSX?

```
Syntax extension for React UI development. 
```

2. What triggers a render cycle?

```
render()
```

3. What is a React Hook?

```
A way to use features without writing a class.
```

4. Which method in a React Component should you override to stop the component from updating?

```
shouldComponentUpdate()
```

5. Which method in a React Component is called after the component is rendered for the first time?

```
componentDidMount()
```

6. What happens when you call setState() inside render() method?

```
Stack overflow error.
```