# From any folder on your Mac:
mkdir courtready-privacy
cd courtready-privacy
# Drop privacy.html into this folder, but rename it index.html so GitHub serves it at the root
mv ~/Downloads/privacy.html index.html

git init
git add index.html
git commit -m "Initial privacy policy"
git branch -M main
gh repo create courtready-privacy --public --source=. --push
# (or do this through github.com if you don't have gh CLI installed)
