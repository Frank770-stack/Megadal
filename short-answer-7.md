### **2️⃣ Short Answer Questions (2 Questions)**

7. **Explain the difference between `position: relative` and `position: absolute` in CSS.**

Write your answer here.
Be as detailed as possible.
You can provide a code snippet using markdown format.

`position: relative` keeps an element in the normal document flow and moves it **relative to its original position**, meaning space is still reserved for it, while `position: absolute` **removes the element from the document flow** and positions it relative to the **nearest positioned ancestor** (or the document if no positioned ancestor exists). This makes `relative` useful for slight adjustments without affecting other elements, whereas `absolute` is ideal for precise positioning inside a container.

```css
.relative-box {
  position: relative;
  top: 20px; /* Moves the element 20px down */
  left: 30px; /* Moves the element 30px to the right */
}

.parent {
  position: relative;
}

.absolute-box {
  position: absolute;
  top: 10px; /* Positioned 10px from the top of .parent */
  left: 50px; /* Positioned 50px from the left of .parent */
}
```
