# real-time-YOLOv5-filter
Modified Wasserstein Cycle GAN for good training and fast predictions in YOLOv5 model.

I decided to omit the other generator and discriminator. It would take way too long and would be inefficient. I know that doesn't really make
it a Cycle GAN anymore, but I still used the architecture, so I decided to keep it.

# Creation
I originally tried to make my own object detector. That proved to be horrible and went wrong because I lack the proper experience for
localization during live video. So I gave up on that. I used YOLOv5 as an alternative. While looking at GANs, I needed something that
would do style transfer and was lightweight，so I settled on the CycleGAN for style transfer which I would modify to make it quicker.

Further, I wanted to use a Wasserstein loss function in order to maximize efficiency. The last time I used BCE, it wasn't very good and
training was kind of unstable.

That brings this all to the FCWGAN, meaning the Fast Cycle Wasserstein GAN. This was a tough project. And I mean really tough. And the result
is something that I'm still not completely satisfied with. Partly because of my styled data. But maybe I'll reuse this project another time.

# Credit
My friend Elliott Cheng gave me his artwork. Thanks for the artworks!
Other than that, photos that I just needed for training are from "I'm something of a painter myself" dataset."
