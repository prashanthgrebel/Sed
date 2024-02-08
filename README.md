# Sed

# insert string / charecter
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
