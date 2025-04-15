## Log contributeur-1

```bash
git clone https://github.com/Elod03/quotes-docs-mkemk-team.git
cd quotes-docs-mkemk-team

git checkout -b contrib1-features
vim docs/index.md
vim README.md
git add docs/index.md README.md
git commit -m "Complete index.md and README.md (Contributor 1)"

touch docs/features.md
vim docs/features.md
git add docs/features.md
git commit -m "Add features.md (Contributor 1)"

vim mkdocs.yml
git add mkdocs.yml
git commit -m "Update mkdocs.yml to add features.md (Contributor 1)"

python -m mkdocs serve
git push origin contrib1-features

git remote add upstream https://github.com/TI204/quotes-docs-mkemk-team.git
git fetch upstream
git checkout main
git merge upstream/main
git push origin main

git checkout -b logs-contributeur-1
vim docs/logs/log-contributeur-1.md

