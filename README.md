# Dog checker

##### Application for classifying dog images using AI according to breed and evaluating if it is actually a dog 

### Running

** THe program accepts 3 arg inputs: **
*dir*: directory where the pictures are placed
*arch*: Model architecture
*dogfile*: file with dog breeds listed

##### The project already contains a dogfile and dir for testing. It is only required to provide the architecture to be used

##### Here is a example. each of the following lines will run the analysis using a different architecture. These commands can be run in batch reuning the file *run_models.sh* and the results will be printed on each arch file like * resnet_pet-images.txt * for resnet

```
python check_images.py --dir pet_images/ --arch resnet  --dogfile dognames.txt > resnet_pet-images.txt
python check_images.py --dir pet_images/ --arch alexnet --dogfile dognames.txt > alexnet_pet-images.txt
python check_images.py --dir pet_images/ --arch vgg  --dogfile dognames.txt > vgg_pet-images.txt
```