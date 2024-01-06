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

<br><br>

# Basic Command:

1. **`git init`**
   - *Usage:* Initializes a new Git repository in the current directory.

2. **`git clone <repository_url>`**
   - *Usage:* Creates a copy of a remote repository on your local machine.

3. **`git git add <filename> ` or `git git add .`**
   - *Usage:* Adds changes to the staging area. The first form adds specific files, and the second form adds all changes.

4. **`git git commit -m "commit message"`**
   - *Usage:* Commits the changes in the staging area with a descriptive message.

6. **`git status`**
   - *Usage:* To check the status of your working directory - which files are modified, untracked, or staged.

7. **`git pull`**
   - *Usage:* Fetches changes from a remote repository and merges them into the current branch.

8. **`git push`**
   - *Usage:* Pushes committed changes to a remote repository.

9. **`git branch`**
   - *Usage:* Lists all local branches and indicates the current branch.

10. **`git checkout <branch_name>` or `git switch <branch_name>`**
   - *Usage:* Switches to the specified branch.

11. **`git merge <branch_name>`**
    - *Usage:* Merges changes from the specified branch into the current branch.

12. **`git log`**
    - *Usage:* Shows the commit history.

13. **`git diff`**
    - *Usage:* Displays the differences between the working directory and the last commit.

14. **`git remote -v`**
    - *Usage:* Lists the remote repositories associated with the current repository.

15. **`git fetch`**
    - *Usage:* Retrieves changes from a remote repository but does not merge them into the local branch.

16. **`git stash`**
    - *Usage:* Temporarily saves changes that are not ready to be committed, allowing you to switch branches.

17. **`git remote add <remote_name> <remote_url>`**
    - *Usage:* Adds a remote repository with the specified name and URL.

18. **`git remote remove <remote_name>`**
    - *Usage:* Removes the remote repository with the specified name.

19. **`git tag`**
    - *Usage:* Lists all tags in the repository.

20. **`git pull origin <branch_name>`**
    - *Usage:* Fetches changes from the remote repository and merges them into the specified branch.

21. **`git push origin <branch_name>`**
    - *Usage:* Pushes committed changes to the specified branch of the remote repository.

22. **`git branch -d <branch_name>`**
    - *Usage:* Deletes the specified local branch.

23. **`git log --oneline`**
    - *Usage:* Displays a compact, one-line representation of the commit history.

24. **`git reset <filename>`**
    - *Usage:* Unstages the changes for the specified file while keeping the modifications in the working directory.

25. **`git config --global user.name "Your Name"`**
    - *Usage:* Sets your global Git username.

26. **`git config --global user.email "your.email@example.com"`**
    - *Usage:* Sets your global Git email.
