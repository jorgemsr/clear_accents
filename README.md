# Clear accents repository

## ./src/generate_example_tree.sh
This script generates an example tree on the _"workspace"_ folder

*Example:*
* André_Almeida
  * test_1
    * one.txt
  * test_2
    * two.txt
  * test_3
    * three.txt
* João_Gonçalves
  * test_1
    * one.txt
  * test_2
    * two.txt
  * test_3
    * three.txt
* Ruben_José
  * test_1
    * one.txt
  * test_2
    *two.txt

## ./src/clear_accents.sh
This script generates a special tree in _"no_accent_folder"_ inside _"workspace"_.

The tree should be exactly the same as inside _"workspace"_ until the last folder level where it is replaced by a symbolik link.

All path and symbolik link should be accent free. 

*Example:*
* Andre_Almeida
  * test_1 -> ../André_Almeida/test_1
  * test_2 -> ../André_Almeida/test_2
  * test_3 -> ../André_Almeida/test_3
* Joao_Goncalves
  * test_1 -> ../João_Gonçalves/test_1
  * test_2 -> ../João_Gonçalves/test_2
  * test_3 -> ../João_Gonçalves/test_3
* Ruben_Jose
  * test_1 -> ../Ruben_José/test_1
  * test_2 -> ../Ruben_José/test_2