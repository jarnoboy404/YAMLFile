# YAMLFile

Loading from resources
```java
@Override
public void onEnable() {
    YAMLFile file = new YAMLFile("Settings.yml", this);
    file.loadDefaultFile();

    file.set("Cookies", true);
    file.saveFile();
}
```
Creating file without loading from resources
```java
@Override
public void onEnable() {
    YAMLFile file = new YAMLFile("Settings.yml", this);
    file.loadFile();

    file.set("Cookies", true);
    file.saveFile();
}
```
