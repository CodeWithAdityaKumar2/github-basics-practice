# Hii Everyone


2. **GitHub par jayein:** Jaise hi aap GitHub open karenge, aapko ek yellow bar dikhega: *"Compare & pull request"*.
3. **PR Create karein:** Us par click karke likhein ki aapne is branch me kya kaam kiya hai, aur "Create pull request" par click kar dein.
4. **Merge PR:** Jab code review ho jaye, toh GitHub UI par hi green rang ka **"Merge pull request"** button dabakar code ko main branch me cloud par merge kar diya jata hai.

---

## 🎯 Phase 2 Practice Tasks (Hands-on Branching)

Apna pichla `github-basics-practice` folder hi open rakhein aur in **6 Tasks** ko complete karein:

### Task 1: Check & Create Branch
* Terminal me check karein ki aap abhi kis branch par hain (`git branch`).
* Ek nayi branch banayein jiska naam ho `feature-styles` aur us branch ke andar switch karein.

### Task 2: Work in Parallel Universe
* `feature-styles` branch ke andar rehte hue, ek nayi file banayein `style.css` aur usme thodi CSS styling likh dein.
* Is file ko stage karein aur commit karein: `git commit -m "Add style.css in feature branch"`.
* Ab wapas `main` branch me switch karein (`git checkout main`) aur apna folder check karein. Kya aapko wahan `style.css` dikh rahi hai? (Nahi dikhni chahiye, kyunki wo sirf doosri branch me hai!)

### Task 3: Local Merging
* `main` branch par rehte hue hi command chalayein: `git merge feature-styles`.
* Ab check karein, kya `style.css` file aapke `main` branch me aa gayi? Is tarah local merge kaam karta hai.

### Task 4: Creating a Remote Feature Branch
* Ek aur nayi branch banayein: `feature-about-page`. Usme switch karein.
* Ek file banayein `about.html` aur use commit kar dein.
* Ab is branch ko GitHub par push karein: `git push origin feature-about-page`. (GitHub par jaakar check karein ki dropdown me do branches dikh rahi hain ya nahi).

### Task 5: The Pull Request (PR)
* GitHub website par jayein, `feature-about-page` ke liye **Create Pull Request** par click karein.
* Description me likhein: *"Adding about page for the project"* aur PR submit kar dein.
* Ab website par hi green button **"Merge pull request"** par click karke use cloud ke `main` branch me merge kar dein.

### Task 6: Cleaning Up & Syncing
* GitHub par merge hone ke baad, wahan "Delete branch" ka option aayega, use daba kar remote branch delete kar dein (standard practice).
* Ab apne local computer ke terminal par aayein, `main` branch me switch karein (`git checkout main`).
* Kyunki cloud par `main` branch aage nikal chuki hai, local computer ko update karne ke liye `git pull origin main` chalayein. Check karein ki `about.html` aapke computer par aa gayi ya nahi.

---

In 6 tasks ko aaram se step-by-step perform kijiye. Kisi bhi step me confusion ho ya koi command samajh na aaye, toh mujhe turant batao.

Jab ye poora ho jaye, toh type karna: **"Phase 2 Done, Move to Phase 3"**!