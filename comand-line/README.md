## FBX2glTF

Installation and use of FBX2glTF in macos

#### installation

1. Move the program into a command directory

```
mv FBX2glTF-darwin-x64 /usr/local/bin/FBX2glTF
```

2. Next, set permissions on it so you can run it:

```
chmod 755 /user/local/bin/FBX2glTF
```

3. Test

```
FBX2glTF -h
```

4. Snipet for converting several files from a directory

```
for i in {1..1003}
do FBX2glTF --binary --draco --verbose \
          --input $i.fbx \
          --output glb/$i.glb
done
```
