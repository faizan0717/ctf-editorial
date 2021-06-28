# information

Q --> 
Files can always be changed in a secret way. Can you find the flag? cat.jpg

sol --> 

use exiftool tool to get the metadata of the image --> exiftool cat.jpg
license in mata data consit of base64 encoded data,decode that --> echo "cGljb0NURnt0aGVfbTN0YWRhdGFfMXNfbW9kaWZpZWR9" | base64 -d