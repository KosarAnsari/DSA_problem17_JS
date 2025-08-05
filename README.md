# Day 17 - 21 Day DSA Challenge 🚀

## 📝 Problem Statement
Write a function that takes a string as input and returns the character with the highest frequency of occurrence in the string.

Example:

Input:  "Hello Worlddddd" Output: 'd'

---

## 💻 Approach
✅ Used a JavaScript object as a **hash map** to store the frequency of each character.  
✅ Iterated through the string and updated the map for every character.  
✅ Traversed the map to find the character with the highest frequency count.  
✅ Returned the character with the maximum occurrence.

---

## 🔑 Key Learnings
- How to use a hash map (object) in JavaScript to efficiently count the frequency of elements.
- Iterating over key-value pairs to determine maximum/minimum conditions.
- This problem helps build a strong foundation for many string-related DSA problems.

---

## 📌 Code
```javascript
function maxOcc(str){
    let map = {};
    str.split('').forEach(element => {
        map[element] = map[element] ? map[element] + 1 : 1;
    });

    let max = 1;
    let char = str[0];
    for (let k in map){
        if (map[k] > max){
            max = map[k];
            char = k;
        }
    }
    return char;
}

let res = maxOcc("Hello Worlddddd");
console.log(res); // Output: d


---

🙌 Connect with Me!

If you’re also working on DSA or interested in collaborative learning, let’s connect on LinkedIn!

#100DaysOfCode #DSA #JavaScript #CodingChallenge #CodeNewbie #DailyCoding #Programming

