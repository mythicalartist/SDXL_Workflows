### Things you wish you knew when you started with SDXL and Comfy UI

___________________

1. ***There is no ideal and magical workflow***  
   This is perhaps the most important idea. There are tons of workflows out there with hundreds of nodes that are capable of doing the most arcane things. However, for creating the most appealing images you do not need most of that. Hence, keep the following in mind.
   1. **There is an ideal pipeline for every image** which is unique to that image. Your goal is to approach that ideal.  
   2. **The most complicated pipeline is not necessarily the best pipeline**, hence starting with a very complicated pipeline that has many elements in it will only make the combinatorial search space larger and make your search more difficult. Hence,
   3. **Start with a simple basic pipeline**, and then modify it appropriately. Once you are getting decent images of what you are looking for, try adding elements to the pipeline and see if things get better. You may have to backtrack and remove and add different things. This is the art part. There is no fixed algorithm to finding the ideal global optimum in this search space. 
2. ***Select an appropriate model***  
    You can always start with the base sdxl model. But the community is always adding more. Some models are more adept at generating some types of images. So search for a model and try it out that you think might suite your current image and subject. Trying out various models will get you to understand many of the strengths and weakness of the individual models.  
3. ***Experiment***
   1. **Try different width and height**. Changing the height and width will often change the composition of the image completely and provide unexpected results and new directions in the image. 
   2. **Try unexpected prompts**. Sometimes adding something unexpected in the prompt that you were not looking for can also affect the image in a pleasing way. 
   3. **Try different total and refiner steps**. This is especially important in many of the non-converging samplers. Increasing steps may increase detail or may mess up the image. Fine-tuning the steps will depend on the subject, prompt, model and pretty much everything else.
   4. **Try different cfg**. Same as sampler above. Although the cfg in the refiner step is more important than in the initial sampler. In most cases, the initial sampler cfg can be left anywhere around 7, and you can play around with the steps and cfg of the refiner.
4. ***Don't go crazy on -ve prompts***  
   You can start off without any negative prompts. They constrain the image in many ways. So at the beginning no need to have any constraints. As you see things in your images crop up that you do not want, add them accordingly to your negative prompts. The long list of negative prompts that you see in many of the images are usually not necessary. Only a few of the items in there usually made the images what they are. 

### Other miscellaneous things

1. ***ChatGPT can provide interesting ideas***  
   But in my humble opinion chatgpt provides too elaborate prompts. It tries to be more evocative than necessary. Ask it to be simple and not be too ornate, and it will tone itself down. 
2. ***Midjourney can also provide very good compositions***  
   If you are not getting good compositions ask Midjourney to create something and then use canny or openpose to guide your own image.
3. ***Use Loras***
   Loras can enhance your image in many interesting ways. Use them, but only after you got your basic image down to satisfaction. Same applies to other enhancements like face detailer etc.  
4. ***Learn Python***  
   If possible, and if you do not know it already, learn python. Even if you do not want to code your own custom nodes, just browsing through the code of the existing nodes will provide better understanding of how they work and their strengths and weakness. 


### Still other miscellaneous things

These are things that might change in the near future as the tools around comfy and sdxl and their models mature. But for now...

1. If you do not like inpainting, avoid compositions that show bare hands and feet. SDXL is terrible with hands and feet. 
2. You can try to incorporate sd1.5 and sdxl in the same pipelines to use the wider suite of tools available for sd1.5. But this will require lots of experimentation. Do not assume this will be easy. However, you can get really good results depending on luck and skill.  