# Sed

# insert string / charecter specific line with matching string
 # * Read at beging of file 
```
cat text.txt | sed  '/<regx string>/s/^/<string need to insert>/'    
```
 # * insert/ modify at beging of file
```
sed  -i '/<regx string>/s/^/<string need to insert>/' text.txt
```
 # * Read at End of file
```
cat text.txt | sed  '/<regx string>/s/$/<string need to insert>/'
```
# * insert/ modify at End of file
```
sed  -i '/<regx string>/s/$/<string need to insert>/' text.txt
```
# Delete line with matching string 
 # * Read only
 ```
cat text.txt |sed  '</regx string>/d'
```
# * Insert / Modify
```
sed -i '/<regx string>/d' text.txt
```

# * Read only - Delete a word after macthing beginning of a word in the line 
```
 cat file.txt | sed '/^\<begining  word >/s/<word to replace or delete>//'
```
# * Modify / write - Delete a word after macthing beginning of a word in the line 

```
 sed -i '/^\<begining  word >/s/<word to replace or delete>//' file.txt
```
