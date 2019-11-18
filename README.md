# Snapshot

Stylizing images using a variety of tools:
1. CycleGANs
2. VGG Net
3. Deep Dream

### VGG
Define style loss and content loss
- Style loss
  - Difference in gram matrix between first couple layers
- Content loss
  - Difference in feature vector between last few layers
  

### CycleGANs
Image domain transfer (i.e apples to oranges)
Two GANS
- Gan 1
  - Generator for apples to oranges
  - Discriminator for making sure outputs are oranges
- Gan 2 
  - Generator for oranges to apples
  - Discriminator for making sure outputs are apples
Cycle consistency loss for making sure when translating from an apple to an orange and then that orange to an apple that the apple images are the same
