# CV Anatoly Shakov
### contact me: @ShakovAS Discord: kihanlol


## About me:
This is my second attempt to finish the RS frontend course. My first attempt was in 2024–2025. I also tried the React course last year.

I was introduced to frontend development a few years ago and started learning it as a hobby. At first, I tried some step-by-step tutorials, such as freeCodeCamp, which gave me a basic understanding of HTML and CSS.

I’m looking forward to seeing what has changed in frontend development over the past few years!

### What i learnt before
* HTML
* CSS
* SASS
* JS
* Typescript
* React

### Some code example:

```
const checkUserInput = () => {
  const inputInt = parseInt(input.value);
  if (isNaN(inputInt) || inputInt == false) {
    resultContainer.style.display = "block";
    result.innerText = "Please enter a valid number"
    return
  } else if (inputInt >= 4000) {
    resultContainer.style.display = "block";
    result.innerText = "Please enter a number less than or equal to 3999"
    return
  } else if (inputInt < 0 ) {
    resultContainer.style.display = "block";
    result.innerText = "Please enter a number greater than or equal to 1"
    return
  }
    resultContainer.style.display = "block";
    result.innerText = romanConverter(inputInt);
    return
}


const romanConverter = (input) => {
  const result = [];
  let num = input

  romanNumerical.forEach((item) => {
    while (num >= item[0]) {
      result.push(item[1])
      num -= item[0]
    }
  })
  return result.join('')
}


convertBtn.addEventListener("click",checkUserInput)

input.addEventListener("keyword",(e) => {
  if (e.key === "Enter") {
    checkUserInput()
  }
})
```