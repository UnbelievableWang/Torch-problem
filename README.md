# Torch-problem
These days when runing a torch program suffering things  

WW gave me a C-project torch-pvnet-jiepu and I finally succeed running it.  

1. Opencv Tiff errors.   
This problem occured when I compiled the project at 100% when build target link.It is because my Opencv must be compiled with -D Tiff and cuda.  

2. yaml target errors.   
This problem happened because I'm not good enough at writing cmake file.  

3.torch magma.  
When I completed compiling the project,I took a deep breathe and relax. However, when I executed it. An error jumped out: what()....Magma,meanwhile,  
it required me compiled again with cuda-magma.  
Then    
    conda install cuda-magma102(depends on cuda version)  
This took a long time.  
then 
    python setup.py clean && setup.py install  
