1. suppose you find the following code in a legacy production codebase. How would you refactor it? 

before:

```js
 getReferrers = function (user_list) {
  user_list = JSON.parse(JSON.stringify(user_list))
  user_list2 = [];
  for (i = 0; i < user_list.length; i++) {
    user_list[i].referrer = user_list.find(function (x) {
      if (x.id == user_list[i]["referrerId"]) {
        return true;
      }
    })
    user_list[i].referrer = user_list[i].referrer && user_list[i].referrer.name || null;
    user_list2.push(user_list[i])
  }
  return user_list2
}
```

after:



Sample input:
```
[
  { id: 1, referrerId: 2, name: "Joe" },
  { id: 2, referrerId: null, name: "Jane" },
  // ... big array of users
]
```


2. Please provide a brief explanation of the difference between `==` and `===`. 


3. What best practices do you consider vital to keep a maintainable frontend project?

4. How do you usually test your components? (methodology, libraries, …)

5. https://evolany.larksuite.com/docs/docuswbZRbPkUSgB8ZjGsaZuHPd
