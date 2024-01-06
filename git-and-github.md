---


---

<h2 id="notes-on-git-and-github">Notes on Git and Github</h2>
<p>To initialize:<br>
<code>git init</code><br>
adds .git folder [repo]</p>
<p>To clone:<br>
copy the &lt;ssh_url&gt;</p>
<p><code>git clone &lt;ssh_url&gt;</code><br>
adds .git folder<br>
adds remote repo info</p>
<p>Git structure:<br>
working directory<br>
[git add]<br>
index/staging<br>
[git commit]<br>
head<br>
[git push]<br>
remote repository (github)</p>
<p>if not cloned and only init:<br>
<code>git remote add origin &lt;ssh_url&gt;</code></p>
<p><code>git pull</code><br>
copies everything from remote repo to your computer</p>
<p><code>git branch</code><br>
copy of code at point in time, with it’s own separate history from main branch (master)<br>
eg: feature A and B</p>
<p>to create a branch<br>
<code>git branch &lt;feature_a&gt;</code><br>
then switch to that branch<br>
<code>git checkout &lt;feature_a&gt;</code></p>
<p>shorthand (create and switch):<br>
<code>git checkout -b &lt;feature_a&gt;</code></p>
<p><code>git merge &lt;feature_a&gt;</code><br>
merged with master branch<br>
<code>git merge &lt;feature_b&gt;</code><br>
if conflicts arise, git will notify</p>
<p>====================</p>
<p>Git and Github setup<br>
download git<br>
create account on github<br>
link git and github using git bash:<br>
<code>git config --global user.name "Your name here"</code><br>
<code>git config --global user.email "your_email@example.com"</code></p>
<p>check for ssh key<br>
<code>ls ~/.ssh</code><br>
you should see a file name ending in .pub<br>
you might get an error saying ssh folder does not exist<br>
then create an ssh key:<br>
<code>ssh -keygen -t rsa -b 4096 -C "your_email@example.com"</code><br>
copy the ssh key<br>
<code>clip &lt; ~/.ssh/id_rsa.pub</code></p>
<p>go to profile settings in github and add the key<br>
then authenticate using the terminal<br>
<code>ssh -T git@github.com</code></p>

