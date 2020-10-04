---
title: Vector Addition
author: Ahnaf Shahriar Asif
sort: 3
---

# Vector Addition

এখন আমরা ভেক্টরের যোগ সম্পর্কে জানবো। আমার মনে আছে, ক্লাস নাইনে আমি ভেক্টরের যোগ কীভাবে করতে হয় সেটা জানলেও কেন এমন করা হচ্ছে এবং আসলে যোগ করলে জিনিস টা কি হয় সেটা ফিল করতে পারতাম না। আমি আশা করি আমরা এখানে যতটুকু সম্ভব ফিল করার চেষ্টা করবো জিনিসটা। আর নিচে একটা ভিডিও দিয়ে দিব 3Blue1Brown এর, আশা করি ক্লিয়ার হয়ে যাবে। তার আগে একটা জিনিস ক্লিয়ার করি, ভেক্টরের বিয়োগ বলতে আলাদা কিছু নেই। আর ভেক্টরের গুন ভাগ বলতেও কিছু হয় না। (ক্রস প্রোডাক্ট আর ডট প্রোডাক্ট বলতে দুইটা জিনিস আছে, ওগুলো ভেক্টরের গুন না আসলে। ওগুলো অন্য জিনিস, আলাদা আলাদা করে ডিফাইন করা হয়েছে কাজের প্রয়োজনে)। তাই মোটামুটি মাথায় এটা রেখে দিও, ভেক্টরের যোগ আর স্কেলিং ছাড়া আর কিছু হয় না। স্কেলিং জিনিসটা আমরা একটু পর দেখবো। এখন আপাতত যোগ কি সেটা দেখে নেই। 

যোগ শেখার আগে আমরা কিছু নোটেশন জেনে নেই। এগুলো বোঝার মতো তেমন কিছু না। জাস্ট কোনটা কি সেটা বোঝানোর জন্য ব্যাবহার করা হয়। যেমন কোনো একটা ভেক্টরের হেড যদি $$(a, b)$$ তে থাকে তাহলে সেই ভেক্টরটিকে $$ \begin{bmatrix}a\\b\end{bmatrix} $$ এভাবে প্রকাশ করা হয়। আর একটা ভেক্টরকে চেনার জন্য আমরা ভেক্টরকে কোনো একটি ভ্যারিয়েবল দিয়ে প্রকাশ করি। যেমন কোনো অজানা সংখ্যাকে x ধরে নেই, বা কোনো রেখাকে AB ধরে নেই, তেমনি একটা ভেক্টর এভাবে প্রকাশ করা হয়ঃ $$\overrightarrow{A}$$। অর্থাৎ, একটি ভেক্টরের নাম যদি আমরা A দেই, তাহলে তার উপরে একটা তীরচিহ্ন দিয়ে দেই। যাতে কেউ যখন এটি দেখে, সে বুঝতে পারে যে A একটা ভেক্টর। এর আর আলাদা কোনো সিগনিফিকেন্স নেই। আর আমরা যখন $$\left\lvert \overrightarrow{A} \right\rvert$$ নেই, এটার মানে আমরা শুধু $$\overrightarrow{A}$$ এর মানটুকু নিচ্ছি, দিক নিয়ে চিন্তা করছিনা। 

যাই হোক। আপাতত এটুকু জানলেই হবে। এখন, ধরি দুইটি ভেক্টর $$\overrightarrow{A}$$ এবং $$\overrightarrow{B}$$। আমরা যদি ভেক্টরদুটি যোগ করি, তাহলে নতুন একটা ভেক্টর পাবো, ধরে নিচ্ছি সেটা $$\overrightarrow{C}$$। অর্থাৎ, $$\overrightarrow{A} + \overrightarrow{B} = \overrightarrow{C}$$। এখন, দুটি ভেক্টরের যোগ বলতে আসলে কী বোঝায়? কী বোঝানো উচিৎ? এভাবে চিন্তা করো। প্রথমে আমরা $$\overrightarrow{A}$$ যেদিকে পয়েন্ট করছে, সেদিকে $$\left\lvert \overrightarrow{A} \right\rvert$$ পরিমান যাবো। তারপর সেখান থেকে $$\overrightarrow{B}$$ যেদিকে পয়েন্ট করছে সেদিকে $$\left\lvert \overrightarrow{A} \right\rvert$$ পরিমান যাবো। তাহলে আমরা যেখানে গিয়ে পৌঁছাবো সেটিই আমাদের $$\overrightarrow{C}$$ এর হেড। মূলবিন্দু থেকে ওই পয়েন্টে তীরচিহ্ণ টানলে আমরা যে ভেক্টর পাবো সেটিই $$\overrightarrow{C}$$। এটি খুবই গুরুত্বপূর্ন। না বুঝলে আরেকবার চিন্তা করে দেখো। নিচের ছবিটিও একটু ভালো করে খেয়াল করো।

<center>
  <img src="{{site.baseurl}}/assets/images/vector_addition.PNG" alt = "vector addition">
</center>

এটি ফিল না করতে পারলে আবারও দেখো। আমরা চাইলে $$\overrightarrow{A}$$ এর হেডে $$\overrightarrow{B}$$ এর টেইল লাগাতে পারবো, যেহেতু ভেক্টরের মান আর দিক ঠিক রেখে যেখানে খুশি সেখানে নাড়াচাড়া করা যায়। এখন একটা মজার জিনিস চিন্তা করো, উপরের ছবিতে আমরা যে $$\overrightarrow{A}$$ আর $$\overrightarrow{B}$$ নিচ্ছি, এরাও কিন্তু নিজেরা দুইটি করে ভেক্টরের যোগফল। নিচের ছবি দেখো, ক্লিয়ার হবে।

<center>
  <img src="{{site.baseurl}}/assets/images/vector_addition_2.PNG" alt = "vector addition">
</center>

অর্থাৎ এখানে আমরা দেখতে পাচ্ছি, $$\overrightarrow{A} = \overrightarrow{X_1} + \overrightarrow{Y_1}$$ এবং $$\overrightarrow{B} = \overrightarrow{X_2} + \overrightarrow{Y_2}$$। একই ভাবে বলতে পারবো $$\overrightarrow{C} = \overrightarrow{X_3} + \overrightarrow{Y_3}$$। এখন, এটা থেকে ইন্টারেস্টিং কিছু জিনিস বের করবো আমরা। আমি প্রথমে বলেছিলাম, $$\overrightarrow{C}$$ পাওয়ার জন্য আমাদের প্রথমে $$\overrightarrow{A}$$ এর দিকে $$\left\lvert \overrightarrow{A} \right\rvert$$ পরিমান যেতে হবে, তারপর সেখান থেকে $$\overrightarrow{B}$$ এর দিকে $$\left\lvert \overrightarrow{B} \right\rvert$$ পরিমান যেতে হবে। এখন আমরা $$\overrightarrow{A}, \overrightarrow{B}$$ গুলোকে ভেঙে লিখেছি। $$\overrightarrow{A}$$ এর দিকে $$\left\lvert \overrightarrow{A} \right\rvert$$ পরিমান যাওয়ার মানে কিন্তু মূলত প্রথমে $$\overrightarrow{X_1}$$ তারপর $$\overrightarrow{Y_1}$$ যাওয়া। আর $$\overrightarrow{B}$$ যাওয়ার মানে আসলে $$\overrightarrow{X_2}$$ গিয়ে তারপর $$\overrightarrow{Y_2}$$ যাওয়া। আবার একটা ছবি দেখো নিচে। 

<center>
  <img src="{{site.baseurl}}/assets/images/vector_addition_3.PNG" alt = "vector addition">
</center>

মূলত আমরা প্রথমে $$\overrightarrow{A}$$ তারপর $$\overrightarrow{B}$$ যাওয়া যে কথা, প্রথমে $$\overrightarrow{X_1}$$ গিয়ে তারপর $$\overrightarrow{Y_1}$$, তারপর $$\overrightarrow{X_2}$$, তারপর $$\overrightarrow{Y_2}$$ যাওয়াও একই কথা। বা সাজিয়ে বললে আমরা প্রথমে $$\overrightarrow{X_1}$$ , তারপর $$\overrightarrow{X_2}$$, তারপর $$\overrightarrow{Y_1}$$, তারপর $$\overrightarrow{Y_2}$$ যাওয়াও সেইম কথা। না বুঝলে ছবি দেখো নিচে। 

<center>
  <img src="{{site.baseurl}}/assets/images/linear_vector_addition.PNG" alt = "vector addition">
</center>

এখন একটা সুন্দর ক্যাচ দেখো। আমরা আগে ধরে নিয়েছিলাম $$\overrightarrow{C} = \overrightarrow{X_3} + \overrightarrow{Y_3}$$। এখন নিচে দেখো। 

$$\begin{aligned} 

\overrightarrow{C} &= \overrightarrow{A} + \overrightarrow{B} \\
&= \overrightarrow{X_1} + \overrightarrow{Y_1} + \overrightarrow{X_2} + \overrightarrow{Y_2} \\
&= \overrightarrow{X_1} + \overrightarrow{X_2} + \overrightarrow{Y_1} + \overrightarrow{Y_2} 

\end{aligned}$$

অর্থাৎ, আমরা দেখতে পাচ্ছি, $$\overrightarrow{X_3} = \overrightarrow{X_1} + \overrightarrow{X_2}$$ এবং $$\overrightarrow{Y_3} = \overrightarrow{Y_1} + \overrightarrow{Y_2}$$ তার মানে আমরা আরও একটা জিনিস কিন্তু বলতে পারছি, নিচের ইকুয়েশনটা দেখো। 

$$\begin{aligned} 

\overrightarrow{C} &= \overrightarrow{A} + \overrightarrow{B} \\ \\
&=  \begin{bmatrix}X_1\\Y_1\end{bmatrix}  +  \begin{bmatrix}X_2\\Y_2\end{bmatrix}  \\ \\
&=  \begin{bmatrix}X_1+X_2\\Y_1+Y_2\end{bmatrix} \\ \\
&=  \begin{bmatrix}X_3\\Y_3\end{bmatrix} 
\end{aligned}$$

অসাধারন, তাই না? :wink:

যাই হোক, ভেক্টরের যোগ নিয়ে আমার মনে হয় আর কোনো প্রকার সমস্যা থাকার কথা না। থাকলে আবার পড়ো। আশা করি কোনো সমস্যা থাকবেনা। নিজে নিজে একটু খাতায় এঁকে এঁকে চিন্তা করো। লিনিয়ার এলজেবরার জিনিসগুলো যদি তুমি মনে মনে গ্রাফে ভিজুয়ালাইজ করার মতো দক্ষতা অর্জন করতে পারো, তাহলে তুমি যখন গনিত বা বিজ্ঞানের অনেক ডিপ জিনিস নিয়ে কাজ করবে, তখন প্রচুর সুবিধা পাবে। তোমার অন্য কলিগরা মনে করবেন তুমি ম্যাজিক জানো, অথবা তুমি সুপার ডুপার জিনিয়াস। তবে সত্যি কথা বলতে এগুলো (এবং পরবর্তী বিষয়গুলো) ভিজুয়ালাইজ করা মোটেই কঠিন কিছু না। আমি যদিও এখনও তেমন একটা পারিনা, কিন্তু আশা করি লিখতে লিখতে শিখে ফেলতে পারবো। এই আর্টিকেল এপর্যন্তই। পরবর্তীতে আমরা ভেক্টরের স্কেলিং এবং তারপরের আর্টিকেলে ভেক্টরের বিয়োগ, গুন, ভাগ কেন হওয়া সম্ভব না সেটি দেখবো। সবাইকে ধন্যবাদ :innocent: