# TODO

- [ ] CREATE Template for Articles
- - [ ] Migrate LaTeX Template Settings from overleaf
- [ ] CREATE Template for SLIDES
- [ ] CREATE Template for projects.

[TASK] REPO for QUARTO templates
[ ] CREATE Showcase sample file
[ ] REVIEW https://quarto.org/docs/output-formats/html-basics.html
[ ] REVIEW https://quarto.org/docs/output-formats/all-formats.html
[ ] REVIEW https://quarto.org/docs/extensions/starter-templates.html
[ ] REVIEW https://quarto.org/docs/extensions/formats.html
[ ] REVIEW https://quarto.org/docs/journals/
[ ] REVIEW quarto env from Andrew Heiss

NTS1: When adding styles directories to this repo you should only include those that you modified yourself, rather than an ready-made template that was modified with your personal info. If you do so, you will not be in sync with template changes.

[ ] CREATE init new repo

```plaintext
./quarto-templates/  
    |-/_journals/{journal-sty}
    |-/_books/{book-sty}/
    |-/_syllabi/{syllabus-sty}/
    |-/_slides/{slide-sty}/
    |-/_manuscripts/{manuscript-sty}/
    |-/_websites/{website-sty}/
    |-.gitignore
    |-README.md
    |-LICENSE

../arena-sty/
    |-.quartoignore
    |-README.md
    |-LICENSE
    |-template.qmd
    |-_extensions/
        |-lexconf/
        |-_extension.yml
        |-theme.scss
        |-logo.png
        |-title.png
```


```Shell
mkdir quarto-templates
touch newfile.txt
git init 
git add .
git commit -m ""
gh create repo 
git push

# USAGE
## Once on GitHub template repo can be instantiated with the following command:

```Shell
cd "/project_dir"
quarto use template mauricimm7/quarto-templates/_journals/arena24
```

This command copies the contents of the GitHub repository at `https://github.com/mauriciomm7/coolproject` to the local system (excluding selected files as discussed above).

Note that the above commands will create a brand new article with default contents. In some cases you may want to use a Journal format in an existing document or project without copying the entire template. In that case you can just add the format extension by itself. For example:

```SHELL
quarto add quarto-journals/acm
quarto add quarto-journals/plos
```

