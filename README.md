# Handwritting characters database

This offline character database was obtained from the UNIPEN online handwriting database [1]. 

To generate this new database, the trajectories obtained from the original UNIPEN online handwritting database was used. Variable-thickness strokes are used depending of the original resolution of the characters to ensure that all final characters have similar thickness. The images from each available category (i.e. different types of alphabet characters) are generated: uppercase, lowercase, digits and punctuation marks. These generated images are resized to 64x64 pixels without changing their aspect ratio. Finally, the generated images are curated manually, one by one, to make sure that they are assigned to their correct category and are human-legible.

This database contains 93 categories and a total of 62,382 image characters in grayscale organized in 93 folders, one for each different character. The folder name are assigned using the ascii numeric code of the character. 


## Characters included in the database
```
! # $ % & ( ) * + , - . / 0 1 2 3 4 5 6 7 8 9 : ; < = > ? @
A B C D E F G H I J K L M N O P Q R S T U V W X Y Z ] ^ _ `
a b c d e f g h i j k l m n o p q r s t u v w x y z f | g ~
```

## Data

```
cat curated.tar.gz.01 curated.tar.gz.02 > curated.tar.gz
tar -xvzf curated.tar.gz
```

## Split
In the split directory we provide the Train/Validaton/Test split used.


## Publications that use this database

* J. Sueiras, et al.: "Using Synthetic Character Database for Training Deep Learning Models Applied to Offline Handwritten Character Recognition", Proc. Intl. Conf.Intelligent Systems Design and Applications (ISDA), Springer, 2016.


## Python code

- transformation.ipynb: This notebook contains the code to apply over the database to perform the transformation described in the paper  "Using Synthetic Character Database for Training Deep Learning Models Applied to Offline Handwritten Character Recognition"


## References

[1] Guyon, I. , Schomaker, L., Plamondon, R., Liberman M., Janet, S.: Unipen project of on-line data exchange and recognizer benchmarks. In: 12th Internacional Conference on Pattern Recognition, Vol.2, pp. 29-33. IEEE (1994)

