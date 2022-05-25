---
title: Find Today's Date
tags: date
expertise: beginner
firstSeen: 2022-05-24
---

This snippet will allow you to find today's date and the current time. It uses the following:

Date() - This constructor finds the current date.
today.getHours() – This uses the today variable to display the current hour. This uses a 24-hour clock.
today.getMinutes() – Displays the current minute reading.
today.getSeconds() – Displays the current seconds reading

```js
function todaysDate() {
const today = new Date();

let date = today.getFullYear()+'-'+(today.getMonth()+1)+'-'+today.getDate();
let time = today.getHours() + ":" + today.getMinutes() + ":" + today.getSeconds();

return `Today's date is ${date} and the current time is ${time}.`
}
```

```js
todaysDate(); // 'Today's date is 2022-05-24 and the current time is 11:39:30.
```
