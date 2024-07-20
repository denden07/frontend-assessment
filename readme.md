# filta-exam

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Project structure
```
Excersie 1 and 2 is on the home page
```

### Answer for this question: Explain why the result of ('b' + 'a' + + 'a' + 'a').toLowerCase() is banana
```

The result of ('b' + 'a' + + 'a' + 'a').toLowerCase() is "banana" due to the following:

*'b' + 'a' results in "ba".

*The + + 'a' part is interpreted as + (+'a'), where +'a' converts the string 'a' to a number, which results in NaN (Not-a-Number).

*Therefore, the expression becomes 'b' + 'a' + NaN + 'a', which results in "baNaNa".

*Applying .toLowerCase() converts "baNaNa" to "banana".
```
