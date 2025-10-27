# Dog checker

##### Application for classifying dog images using AI according to breed and evaluating if it is actually a dog 

### Running

**The program accepts 3 arg inputs:** <br />

**dir**: directory where the pictures are placed <br />
**arch**: Model architecture. Options are vgg, resnet and alexnet <br />
**dogfile**: file with dog breeds listed <br />

##### The project already contains a dogfile and dir for testing. It is only required to provide the architecture to be used.

##### Here is an example. each of the following lines will run the analysis using a different architecture. <br /> These commands can be run in batch running the file *run_models.sh* and the results will be <br />printed on each arch file like * resnet_pet-images.txt * for resnet

```sh
python check_images.py --dir pet_images/ --arch resnet  --dogfile dognames.txt > resnet_pet-images.txt
python check_images.py --dir pet_images/ --arch alexnet --dogfile dognames.txt > alexnet_pet-images.txt
python check_images.py --dir pet_images/ --arch vgg  --dogfile dognames.txt > vgg_pet-images.txt
```
