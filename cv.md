# Shakov Anatoly

## A newbie to a frontend developing

## Contacts
 * **telegram** @ShakovAS

## About myself and my coding journey:

I am started coding in a 2020. The first thing i started to learn was a frontend developing so I started with HTML and CSS.It was more a hobby for me and i didnt invest much time in it.
And after i joined telegram chat with a great community it inspired me to take a more serious approach to coding and even consider a developer carrier.

Some code example:

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

This is example of code i wrote for freeCodeCamp task.

====

## Languages:
    * Russian (native)
    * English