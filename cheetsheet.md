#export java class
export CLASSPATH=$CLASSPATH:/home/milowenwen/eclipse/java-oxygen/eclipse/java_libs/hapi-fhir-base-3.2.0.jar

#config git global var
git config --global -e

#show all branches
git branch -a

#delete a local brach
git branch -d <branch_name>

#find current git status
git status

#git switch to branch_1
git checkout branch_1

#show current branch
git branch

#show current change made (in current branch)
git difftool README.md

#show current change made in specifed branch_1
git difftool branch_1 README.md

#show all diff based on two SHA
git difftool 2e26404a91defa2d065b73fb4b8322fb8af1cc31 c8cc65eab7214cc6c7a6dc57c4b08b4c0fa3bd84 

#show README.md diff based on two SHA
git difftool a22d80c1cd0d98f8c69b181b4be8c959bd15b160 c8cc65eab7214cc6c7a6dc57c4b08b4c0fa3bd84 README.md

#show diff between specified SHA and current README.md
git difftool a22d80c1cd0d98f8c69b181b4be8c959bd15b160 README.md

#stage to commit for ALL unstaged files
git add .

#stage to commit for README.md
git add README.md

#commit with msg
git commit -m "Make change 2"

#add remote repo on github
git remote add origin https://github.com/alsomilo/testsetup.git

#remote push
git push -u origin master

#remote pull
git pull -u origin master

#see repo url
git remote show origin

#export algo class ext libs
export CLASSPATH=$CLASSPATH:/home/milowenwen/eclipse/java-oxygen/eclipse/java_libs/algs4.jar

#.gitconfig file
[user]
	name = alsomilo
	email = yuan.wdc@gmail.com
[diff]
        tool = meld
[difftool]
        prompt = false
[difftool "meld"]
        cmd = meld "$LOCAL" "$REMOTE"
[merge]
        tool = meld
[mergetool "meld"]
        cmd = meld "$LOCAL" "$BASE" "$REMOTE" --output "$MERGED"
       #cmd = meld "$BASE" "$LOCAL" "$REMOTE" --output "$MERGED"
       #cmd = meld "$LOCAL" "$MERGED" "$REMOTE" --output "$MERGED"
[mergetool]
        keepBackup = false
[core]
	editor = notepadqq

#resove a conflict
git mergetool

test
