# **Aleksandr Mikhaylov**

---

## **Contact information:**

- **E-mail: alex.mcgee.mail@gmail.com**
- **Telegram: [@ranpu](https://t.me/ranpu)**
- **[LinkedIn](https://www.linkedin.com/in/aleksandr-mikhaylov-3583b0104/)**

---

---

## **Skills and Proficiency:**

- **HTML5, CSS3** *(Beginner)*
- **JavaScript** *(Beginner)*
- **Python** *(Junior)*
- **Adobe Photoshop, CorelDraw** 
- **Git, GitHub**
- **VS Code**

---

## **Code examples:**

**[Count IP Addresses KATA from CODEWARS (JavaScript solution):](https://www.codewars.com/kata/526989a41034285187000de4/javascript)**

```JavaScript
function ipsBetween(start, end){
    start = start.split('.')
    end = end.split('.')
    let diff = []
  
    for (let i = 0; i < 4; i++) {
        start[i] = Number(start[i])
        end[i] = Number(end[i])
        diff.push(start[i] - end[i])
    }
  
    return Math.abs((256**3 * diff[0]) + 
                    (256**2 * diff[1]) +
                    (256 * diff[2]) + diff[3])
  
}
```

**[Range Extraction KATA from CODEWARS (Python solution):](https://www.codewars.com/kata/51ba717bb08c1cd60f00002f/python)**

```Python
def solution(args):
    args += [None]
    final, middle = [], [args[0]]
    
    for x in range(1, len(args)):
        if args[x-1] + 1 != args[x]:
            if len(middle) > 2:
                final += [str(middle[0]) + '-' + str(middle[-1])]
            else:
                final += [str(x) for x in middle]
            middle = [args[x]]
        else:
            middle += [args[x]]
            
    return ','.join(final)
```
---