# first setup
installieren
```
brew install git
```
public ssh-key uz GitHub hinzufügen
testen
```
ssh -T git@github.com
```
account-details setzen
```
git config --global user.name "<GitHub Name>"
git config --global user.email "<email github>"
```
# setup
klonen
```
git clone git@github.com:<user>/<repository>.git
```
# bearbeiten
wählen
```
cd <repository>
```
öffnen
```
code .
```
speichern
```
git add .
git commit -m "ssh Commit"
git push
```
