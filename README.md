linux_reference
===============

```
for f in rasters-2012.cc_*_2013_raster/metadata.json; do cp ${f} ${f}.bk && sed -i 's/stops=%23dae660,%23a8c23f,%2358a373,%23157f99,%23004d70/stops=%237e9e3d,%23a5ad37,%23f5c215,%23c66428,%23a02321/g' $f; done

for FILE in *.jpg; do mv "$FILE" $(echo "$FILE" | sed 's/2_/1_/'); done

# delete all coffee files within the js directory
find js -name '*.coffee' -delete

# Replace all term.description to term.definition in /home/deciob/dev/biodiversity-a-to-z/app
find /home/deciob/dev/biodiversity-a-to-z/app -type f -exec \
 > sed -i 's/term.description/term.definition/g' {} + 


```


### Some ruby-rails stuff

```rb
      debugger
      @user.errors.to_a
```
