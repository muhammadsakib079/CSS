### 🎨 **1. Background Image Handling**
CSS-এ **background-image** ব্যবহারের মাধ্যমে ওয়েবসাইটের ব্যাকগ্রাউন্ডে ইমেজ সেট করা যায়।

#### ✅ **Basic Syntax**
```css
body {
    background-image: url('image.jpg');
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center;
}
```
✔ `background-size: cover;` – ইমেজ পুরো এলাকা কভার করবে।  
✔ `background-repeat: no-repeat;` – ইমেজ রিপিট হবে না।  
✔ `background-position: center;` – ইমেজকে মাঝামাঝি রাখবে।  

#### ✅ **Overlay Effect**
```css
.background {
    position: relative;
}
.background::after {
    content: "";
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: rgba(0, 0, 0, 0.5); /* Dark overlay */
}
```
✔ **ব্যাকগ্রাউন্ড ইমেজের উপর ডার্ক/লাইট লেয়ার তৈরি করা যায়।**

---

### 🎞 **2. CSS Animations**
CSS Animation ব্যবহার করে **smooth effects** তৈরি করা যায়।

#### ✅ **Keyframe Animation**
```css
@keyframes fadeIn {
    0% { opacity: 0; }
    100% { opacity: 1; }
}
.box {
    animation: fadeIn 2s ease-in-out;
}
```
✔ `@keyframes` ব্যবহার করে **কাস্টম এনিমেশন** তৈরি করা হয়।  
✔ `animation: fadeIn 2s ease-in-out;` – ২ সেকেন্ড ধরে **fade-in effect** হবে।

#### ✅ **Hover Effect Animation**
```css
button:hover {
    transform: scale(1.1);
    transition: transform 0.3s ease;
}
```
✔ **মাউস হোভার করলে বোতাম বড় হবে।**

---

### 📐 **3. CSS Grid Layout**
Grid Layout ব্যবহার করে **responsive এবং flexible** লেআউট তৈরি করা যায়।

#### ✅ **Basic Grid Structure**
```css
.container {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 20px;
}
.item {
    background: lightblue;
    padding: 20px;
    text-align: center;
}
```
✔ `grid-template-columns: repeat(3, 1fr);` – **৩টি কলাম তৈরি করবে।**  
✔ `gap: 20px;` – **গ্রিড আইটেমগুলোর মাঝে গ্যাপ রাখবে।**

---

### 📦 **4. CSS Flexbox**
Flexbox ব্যবহার করে **বিভিন্ন কম্পোনেন্ট সহজে সজ্জিত করা যায়।**

#### ✅ **Basic Flexbox Structure**
```css
.container {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
}
```
✔ `justify-content: center;` – **আইটেমগুলোকে অনুভূমিকভাবে মাঝখানে রাখবে।**  
✔ `align-items: center;` – **আইটেমগুলোকে উল্লম্বভাবে মাঝখানে রাখবে।**

#### ✅ **Flex Direction (Row & Column)**
```css
.container {
    display: flex;
    flex-direction: column;
}
```
✔ `flex-direction: column;` – **আইটেমগুলোকে কলামের আকারে সাজাবে।**

---

### 🔄 **5. Transform & Translation**
Transform & Translation ব্যবহার করে **স্কেল, ঘোরানো, সরানো ইত্যাদি করা যায়।**

#### ✅ **Rotate Effect**
```css
.box {
    transform: rotate(45deg);
}
```
✔ `rotate(45deg);` – **আইটেমটি ৪৫ ডিগ্রি ঘুরবে।**

#### ✅ **Translate Effect**
```css
.box {
    transform: translate(50px, 20px);
}
```
✔ `translate(50px, 20px);` – **আইটেম ৫০ পিক্সেল ডানে ও ২০ পিক্সেল নিচে সরবে।**

#### ✅ **Scale Effect**
```css
.box {
    transform: scale(1.5);
}
```
✔ `scale(1.5);` – **আইটেমটি ১.৫ গুণ বড় হবে।**

---

এই **CSS গাইড** আপনাকে **ব্যাকগ্রাউন্ড হ্যান্ডলিং, এনিমেশন, গ্রিড, ফ্লেক্সবক্স ও ট্রান্সফর্ম** সম্পর্কে পরিষ্কার ধারণা দেবে। 🚀