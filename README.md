# AC-kicad-library
Personal KiCAD library for items that don't belong in the KiCAD native repos
## Using in other projects
The best way is to add this library as a submodule in any other project requiring it.
```
cd <other_project>
git submodule add git@github.com:mradamcollins/AC-kicad-library.git 
```
Then add AC-kicad-libarry as a project specific library in Kicad manage libraries tab

### Updating the submodule
Submodules are fixed by nature, to manual update the library use:
```
git submodule update --remote
```

## Using easyeda2kicad scripts
to install:
* cd C:\Users\<username>\Documents\KiCad
```
cd C:\Users\<username>\Documents\KiCad\AC-kicad-library
python3 -m venv .venv
source .venv/bin/activate
pip3 install easyeda2kicad
```
to download models from lcsc
```
cd C:\Users\<username>\Documents\KiCad\AC-kicad-library
 easyeda2kicad --full --lcsc C132562 --output ./AC-kicad-library
 ```
 where --lcsc parameter is their part number