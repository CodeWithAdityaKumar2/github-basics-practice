---

## 🎯 Phase 3 Practice Tasks (Let's Break and Fix It!)

Chaliye intentionally (jaan-boojhkar) ek conflict banate hain aur use khud solve karte hain. Isko step-by-step follow kijiye:

### Task 1: Foundation Taiyar Karein
* Apne `main` branch me aaiye (`git checkout main`).
* Ek nayi file banayein `conflict-test.txt` aur uski pehli line me likhein: `Original Text by Aditya`.
* Ise add aur commit kar dein: `git commit -m "Add conflict-test.txt"`.

### Task 2: Universe A (Branch 1) me Badlav
* Ek naya branch banayein: `branch-one` aur usme switch kar jayein.
* `conflict-test.txt` ko open karein aur us text ko badal kar likhein: `Text edited by Branch One`.
* File ko save karein, add karein aur commit kar dein: `git commit -m "Edit by branch one"`.

### Task 3: Universe B (Branch 2) me Badlav
* Wapas `main` branch par aaiye (`git checkout main`).
* Ab `main` se ek aur naya branch banayein: `branch-two` aur usme switch karein.
* Usi `conflict-test.txt` file ko open karein (yahan abhi original text dikhega). Isko badal kar likhein: `Text edited by Branch Two`.
* File ko save karein, add karein aur commit kar dein: `git commit -m "Edit by branch two"`.

### Task 4: The Conflict (Dhamaka! 💥)
* Wapas `main` branch me aaiye (`git checkout main`).
* Pehle `branch-one` ko main me merge karein: `git merge branch-one`. (Yeh aaram se bina kisi dikkat ke merge ho jayega).
* Ab asli maza aayega. Ab `branch-two` ko bhi main me merge karne ki koshish karein: `git merge branch-two`.
* **Boom!** Terminal me ek error message aayega: `CONFLICT (content): Merge conflict in conflict-test.txt. Automatic merge failed; fix conflicts and then commit the result.`

### Task 5: Resolving the Conflict
* VS Code me `conflict-test.txt` file ko kholein. Aapko wahan conflict markers (`<<<<<<<`, `=======`, `>>>>>>>`) dikhenge.
* VS Code ke buttons ka use karke **"Accept Both Changes"** par click karein taaki dono branches ka text reh jaye.
* Check karein ki saare ajeeb symbols (`<<<`, `===`, `>>>`) gayab ho gaye hain aur sirf saaf text bacha hai.

### Task 6: Completing the Merge
* Terminal me aakar check karein `git status`. Wo kahega ki aap abhi merge process ke beech me hain.
* File ko stage karein: `git add conflict-test.txt`.
* Is merge ko complete karne ke liye commit karein: `git commit -m "Resolve conflict between branch-one and branch-two"`.
* `git log --oneline` chala kar dekhein ki aapka clean history graph ban gaya hai.

---

Yeh 6 tasks aapko real-world me aane wale 90% merge conflicts se darrna band karwa denge. Inhe aaram se kariye. 

Jab aap conflict successfully fix kar lein aur commit ho jaye, toh mujhe reply karein: **"Phase 3 Done, Move to Phase 4"**! Agar beech me kahin atak jao, toh terminal ka error mujhe bhej dena.