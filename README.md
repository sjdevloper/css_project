# css_project

Reference [freeCodeCamp](https://www.freecodecamp.org).

 
### Problem 1
How can I delete a repository on github with an arrow? I would not like to delete my last commit.

#### Answer [reference](https://stackoverflow.com/questions/62707431/how-can-i-delete-a-repository-on-github-with-an-arrow)

An arrow means "gitlink", a SHA1 reference to another repository.
If you have a .gitmodules file in the same repository, that folder would have a '@': submodule, but I suspect it is not the case here
It is best deleted locally:
* git clone
* git rm --cached algortimos-eleicao # no trailing /
* git commit -m "remove gitlink"
* git push 
