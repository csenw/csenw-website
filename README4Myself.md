1. clone the original academic themes and hugo framework
2. locally modify everything
3. create two repositories on github: csenw-website & csenw.github.io. The first one is for hugo source code while the second one is for generated static html files.
4. git remote rm origin (remove remote git for the original code)
5. git remote add https://github.com/csenw/csenw-website.git

6. remove public folder locally
7. add public folder as a submodule of hugo code: git submodule add -f -b master https://github.com/<USERNAME>/<USERNAME>.github.io.git public
8. git push origin master

9. use hugo to generate files in public
10. go to public and git add/commit to the csenw.github.io.
Done.


Daily maintain: 
1. modify code in the folders (such as /layout, /content, etc.)
2. hugo to generate new static html files in publich
3. push origin master in the root folder -> csenw-website
4. goto public folder and push origin master -> csenw.github.io

5. Post a news thread: hugo new post/TCYB-accepted.md