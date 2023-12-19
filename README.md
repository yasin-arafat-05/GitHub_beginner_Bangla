<h1 align="center">
  গিট এবং গিটহাব
</h1>

<!-- What is git -->
<p> 
<h2> গিট কি? (What is Git?)</h2>
গিট হলো একটি Open-source ভার্সন কন্ট্রোল সিস্টেম যা দিয়ে আমরা একটি প্রজেক্টের ফাইল গুলোর পরিবর্তন ট্র্যাক করতে পারি। গিট ২০০৫ সালে লিনাক্স কার্নেলের জন্য প্রকাশ করা হয় যার স্রস্টা Linus Torvalds.
</br>
<a href="https://en.wikipedia.org/wiki/Git">Source Link</a>
</p>

<!-- Version-Control System -->
<p> 
<h2>ভার্সন কন্ট্রোল কি? (What is version control)</h2>
ভার্সন কন্ট্রোল কি? আমাদের কেন ভার্সন কন্ট্রোল দরকার? (What is version control and why we should care?) >> যে পদ্ধতিতে কোনও প্রজেক্টের ফাইলগুলোর পরিবর্তন ট্র্যাক করে রাখা হয় যাতে করে আমরা পরে দরকারে আগের নির্দিস্ট ভার্সনে যেতে পারি তাকে ভার্সন কন্ট্রোল (Version Control System বা VCS) বলে। গিট প্রায় যেকোনো ফাইলের পরিবর্তন গুলো ট্র্যাক করে রাখতে পারে।
</br>

<a href="https://en.wikipedia.org/wiki/Git">Source Link</a>
</p>


<!-- Starting with git -->

<p>
<h1>
  Starting with git:
</h1>
যেই ফোল্ডাকে গিট এ অ্যাড করতে চাই সেই folder এর মধ্যে প্রবেশ করে, r8 button এ ক্লিক করে open git base here এ ক্লিক করবো।
শুরুতে username and gmail set করতে হবে। কারণ কোন কিছু change করলে কে change করেছে globallay সেইটা দেখার জন্য username and gmail configuration করতে হবে ।

GitHub এর কাজ হলো কোন repository create করা থাকলে তার cloning করতে পারি । cloning এর মাধ্যমে server থেকে ডাটা আমাদের computer আসবে । আর না করা থাকলে আমরা new repository create করতে পারি । যেহেতু, আমরা github এ নতুন একটা ফোল্ডার insert করতেছি । তাই শুরুতে আমদের কে initialization করতে হবে । git init command এর মাধ্যমে । git init command ব্যবহার করলে, সেই folder এর hidden file হিসেবে ৩টা file crate হবে । যার মধ্যে .git file এ সবকিছু থাকবে । hidden file দেখার জন্য ls -lart command দিতে হবে।

এখন সেই folder এ যদি index.html নামে একটি নতুন file খুলি । তারপর git status command run করি । তাইলে আমরা এইখানে, কোন commits থাকবে না এবং untrack file গুলো দেখতে পারবো ।

এখানে, untrack file,Staging area, commit কি?

Untracked: এর মানে হলো git এর মাধ্যমে আমরা যেইসব file কে observe করতেছি কিন্তু এদের কে track করতেছি না । আমদের কে সব file track করার দরকার হবে না ।যেমনঃ C++ প্রোগ্রাম রান করলে আরো নতুন ২টা file তৈরি হয় । যাদেরকে আমাদের track করার প্রয়োজন হয় না । তাই আমরা শুধু .c ফাইলটাকে track করবো । কোন ফাইল track করার জন্য একে staging area এ নিয়ে যাবো। staging area তে আমরা সেইসব ফাইলকে নিয়ে যায় যারা commit এ যাবে । Unmodified এ গেলে আমাদের ফাইল git এর মধ্যে চলে গেছে । এখন ইচ্ছা করলে git থেকে আমরা কোন ফাইলকে remove করতে পারি বা কোন পরিবর্তন করার দরকার হলে তা করি এবং তা আবার staging area দিয়ে commit এর মাধ্যমে Unmodified এ চলে যায়।

Git add file_name এটা দিয়ে কোন ফাইল কে staging area তে নিয়ে যাওয়া হয় । এখন git status command দিলে সেই ফাইলটাকে আমাকে commits করার জন্য বলা হবে ।
এখন, জিনিস পাতি একটু complex,...
Git commit command দিব দেন i বাটন প্রেস করে Initial Commit লিখবো, দেন :wq দেন প্রেস enter, commit done .
এখন, git status command দিলে, (এখন পযন্ত যা commit হয়েছে তা github এ আছে )।
</p>

<!-- 
<p>
  
<ul>
  <li>মডিফাইড – Modified</li>
  <li>স্টেজড – Staged</li>
  <li>কমিটেড – Committed</li>
</ul>  

</p>

-->
